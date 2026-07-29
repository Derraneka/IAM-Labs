# Meridian Defense Solutions — Identity & Access Management

A working Microsoft Entra ID environment built and operated end-to-end: architecture, runbooks, policy-as-code, and audit evidence for a simulated defense contractor.

---

## The organization

**Meridian Defense Solutions (MDS)** is a fictional 250-person DoD prime/subcontractor headquartered in San Antonio, TX, with remote engineering staff. CUI is in scope. The organization operates under NIST SP 800-171 obligations and is working toward CMMC Level 2. Government-facing staff are required to authenticate with CAC/PIV.

Every artifact in this repository is written as work performed for MDS — access requests, incidents, projects, and audit deliverables — rather than as isolated exercises. The intent is to demonstrate how an IAM analyst/engineer actually operates a tenant, not just which buttons exist in the portal.

**This is a personal lab environment.** It is not connected to, derived from, or representative of any employer's environment. All users, data, and business context are synthetic.

---

## Environment

| Component | Detail |
|---|---|
| Identity provider | Microsoft Entra ID |
| Tenant | Meridian Defense Solutions (cloud-only at present; hybrid in Phase 2) |
| Licensing | Entra ID Free baseline; P2 and Entra ID Governance trials activated per phase |
| Automation | Microsoft Graph PowerShell SDK, Terraform (`azuread`), GitHub Actions |
| Monitoring | Log Analytics, KQL, Azure Workbooks |
| Compliance tooling | ScubaGear (CISA SCuBA), Maester, EIDSCA |

All tenant identifiers, object IDs, and domains in screenshots and documentation are redacted or replaced with the sanitized domain `meridiandefense.onmicrosoft.com`.

---

## Repository structure

```
├── 00-tenant-foundation/        Tenant standup, admin model, identity data model
├── 01-analyst-operations/       Access requests, triage, JML runbooks
├── 02-hybrid-identity/          AD DS, Entra Connect Sync, break/fix
├── 03-application-integration/  SAML, OIDC, SCIM, app risk review
├── 04-conditional-access/       CA framework, phishing-resistant MFA, CBA
├── 05-identity-governance/      PIM, entitlement management, access reviews, LCW
├── 06-automation-and-iac/       PowerShell module, Terraform, CI/CD
├── 07-monitoring-and-response/  KQL library, Identity Protection, IR playbooks
├── 08-federal-icam/             SCuBA, NIST 800-53 / 800-63 mapping, Zero Trust
├── runbooks/                    Standalone operational SOPs
├── scripts/                     Reusable Graph PowerShell toolkit
├── policy-as-code/              Exported CA policies, Terraform, Bicep
└── docs/
    ├── architecture/
    ├── standards/
    └── compliance/
```

---

## Runbook index

| ID | Title | Status |
|---|---|---|
| RB-001 | Break-glass emergency access accounts | Complete |
| RB-002 | Sign-in failure triage | In progress |
| RB-003 | Access request fulfillment | Planned |
| RB-004 | Joiner | Planned |
| RB-005 | Leaver | Planned |
| RB-006 | Mover | Planned |
| RB-007 | Entra Connect sync troubleshooting | Planned |
| RB-008 | SAML signing certificate rollover | Planned |
| RB-009 | Conditional Access change management | Planned |
| RB-010 | Compromised identity response | Planned |

---

## Lab index

### Phase 0 — Tenant Foundation
- [x] **0.1 — Tenant standup and administrative tiering** → [writeup](00-tenant-foundation/README.md)
- [ ] 0.2 — Naming standards and identity data model
- [ ] 0.3 — Synthetic organization population

### Phase 1 — Analyst Operations
- [ ] 1.1 Access request fulfillment · 1.2 Authentication methods modernization · 1.3 Sign-in triage
- [ ] 1.4 Group-based licensing · 1.5 Joiner · 1.6 Leaver · 1.7 Mover

### Phase 2 — Hybrid Identity
- [ ] 2.1 AD DS deployment · 2.2 Entra Connect Sync · 2.3 Sync break/fix · 2.4 Cloud Sync · 2.5 Hybrid join

### Phase 3 — Application Integration
- [ ] 3.1 Gallery SAML · 3.2 Custom SAML · 3.3 OIDC/OAuth · 3.4 SCIM outbound
- [ ] 3.5 API-driven inbound provisioning · 3.6 App risk inventory · 3.7 B2B and cross-tenant access

### Phase 4 — Conditional Access & Zero Trust
- [ ] 4.1 Persona-based CA framework · 4.2 Safe deployment · 4.3 Phishing-resistant MFA
- [ ] 4.4 Certificate-based authentication (CAC/PIV) · 4.5 Device compliance · 4.6 Session controls & CAE · 4.7 CA as code

### Phase 5 — Identity Governance
- [ ] 5.1 PIM · 5.2 Entitlement management · 5.3 Access reviews · 5.4 Lifecycle workflows · 5.5 Separation of duties

### Phase 6 — Automation & Identity-as-Code
- [ ] 6.1 PowerShell module · 6.2 Terraform · 6.3 CI/CD with workload identity federation · 6.4 Compliance reporting

### Phase 7 — Monitoring, Detection & Response
- [ ] 7.1 Log pipeline & KQL · 7.2 Identity Protection · 7.3 IR playbook · 7.4 Attack path review · 7.5 Posture dashboard

### Phase 8 — Federal ICAM
- [ ] 8.1 CISA SCuBA assessment · 8.2 Maester continuous testing · 8.3 NIST 800-53 mapping
- [ ] 8.4 NIST 800-63-3 assurance levels · 8.5 Zero Trust gap assessment · 8.6 ICAM program design

---

## Standards and design documents

- [Administrative tiering model](docs/standards/admin-tiering-model.md)
- Naming and attribute standard *(pending — Lab 0.2)*
- Conditional Access framework *(pending — Lab 4.1)*

---

## Author

Derra Hewlett — USAF veteran (2014–2024), MS Cybercrime
