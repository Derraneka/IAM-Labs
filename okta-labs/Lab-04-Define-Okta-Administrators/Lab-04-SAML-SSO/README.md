# SAML Single Sign-On (SSO)

## Objective
Configure Single Sign-On using the SAML 2.0 protocol.

## Technologies Used
- Okta
- SAML 2.0

## Skills Practiced
- SAML
- Federation
- Single Sign-On
- Enterprise Applications

## Tasks Completed
- Created a SAML application
- Configured SAML settings
- Configured attribute statements
- Assigned users
- Verified successful SSO authentication

## Screenshots
## 1. Accessed the Applications Console

Navigated to **Applications → Applications** to begin creating a new SAML application.

![Accessed the Applications Console](screenshots/1.png)

---

## 2. Selected SAML 2.0 Integration

Created a new application integration using the **SAML 2.0** sign-in method.

![Selected SAML 2.0 Integration](screenshots/2.png)

---

## 3. Configured General Application Settings

Named the application **SAML Test Application**.

![Configured General Application Settings](screenshots/3.png)

---

## 4. Configured Core SAML Settings

Configured the **Single Sign-On URL**, **Audience URI**, **Name ID Format**, and **Application Username**.

![Configured Core SAML Settings](screenshots/4.png)

---

## 5. Opened Application Assignments

Navigated to the **Assignments** tab.

![Opened Application Assignments](screenshots/5.png)

---

## 6. Assigned a User to the Application

Assigned a user to the SAML Test Application.

![Assigned a User](screenshots/6.png)

---

## 7. Reviewed SAML Metadata

Viewed the **Metadata URL**, **Sign-On URL**, **Issuer**, and **Signing Certificate**.

![Reviewed SAML Metadata](screenshots/7.png)

---

## 8. Assigned a Group to the Application

Selected **Assign → Assign to Groups**.

![Assigned a Group](screenshots/8.png)

---

## 9. Granted Group Access

Assigned the **Marketing** group to the SAML application.

![Granted Group Access](screenshots/9.png)

---

## 10. Reviewed Attribute Statements Configuration

Opened the **Attribute Statements** section for SAML claims configuration.

![Reviewed Attribute Statements](screenshots/10.png)

---

## 11. Verified Application in the End User Dashboard

Confirmed the application appeared in the Okta End User Dashboard after assignment.

![Verified End User Dashboard](screenshots/11.png)

---

## 12. Successfully Initiated SAML Single Sign-On

Launched the application and verified successful redirection to the configured **Single Sign-On URL**.

![Successful SAML Sign-On](screenshots/12.png)

---

## 13. Verified Successful Authentication in the System Log

Confirmed a successful **User Single Sign-On to App** event in the Okta System Log.

![Verified System Log](screenshots/13.png)

## Key Takeaway
This lab demonstrates federated authentication using the SAML 2.0 protocol to provide secure Single Sign-On.
