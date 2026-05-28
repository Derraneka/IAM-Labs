# Lab-03: Organize Users With Groups

## Overview

Completed the Okta Workforce Identity Cloud skill badge: **Organize Users With Groups**.

This lab focused on creating and managing groups, automating user assignments, assigning administrative roles, and using Okta Expression Language to dynamically manage access.

---

## Skills Demonstrated

- Group Creation
- Manual Group Assignment
- Dynamic Group Assignment
- Group Rules
- Group-Based Access Control (GBAC)
- Administrative Role Assignment
- Okta Expression Language
- User Attribute Evaluation

---

## Key Concepts Learned

### Manual Group Assignment

Best used for:

- Administrative groups
- Privileged access groups
- Special access requests

### Dynamic Group Assignment

Automates group membership based on:

- User attributes
- Existing group membership
- Expression Language conditions

---

## Group Rule Examples

### Assign Non-Employees

```text
user.userType != "Employee"
```

Purpose:

Assign Contractors and Partners to an External Users group.

---

### Assign High Security Users

```text
user.securityLevel >= 8
```

Purpose:

Assign users with elevated security clearances to a High Security group.

---

### Assign Suspended Users

```text
user.getInternalProperty("status") == "SUSPENDED"
```

Purpose:

Automatically identify suspended accounts.

---

### Assign Sales Department Users

```text
user.department == "Sales"
```

Purpose:

Automate membership in Sales-related groups.

---

## Administrative Access Management

Administrative roles can be assigned directly to groups to simplify administration and ensure consistent permissions across teams.

Examples:

- Help Desk Administrator
- Application Administrator
- Read-Only Administrator
- Group Administrator

---

## Lessons Learned

- Group rules reduce manual administrative effort.
- String comparisons are case-sensitive.
- Internal user statuses require `getInternalProperty("status")`.
- Administrative access should be tightly controlled.
- Group-based administration improves scalability.
- Dynamic group membership supports automated access management.

---

## Badge Earned

🏆 Organize Users With Groups

Topics Covered:

- Group Management
- Group Rules
- Okta Expression Language
- Administrative Roles
- Dynamic User Assignment
- Access Automation

---

## Career Relevance

This lab strengthened practical Identity and Access Management (IAM) skills related to:

- User Lifecycle Management
- Access Governance
- Role-Based Access Control (RBAC)
- Identity Security
- Okta Administration
