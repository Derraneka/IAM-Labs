# Okta Org2Org User Provisioning with SCIM, SAML, and Custom Attribute Mapping

## Overview

This project demonstrates a complete Identity and Access Management (IAM) lifecycle using Okta Org2Org, SAML 2.0, and SCIM provisioning. The lab focuses on automating user provisioning, synchronizing profile attributes between two Okta organizations, and validating automated deprovisioning.

The environment was built entirely within Okta Integrator Free Plan organizations to simulate a real enterprise identity integration.

---

# Objectives

- Configure an Okta Org2Org application
- Enable SCIM provisioning
- Configure API integration using an Okta API token
- Configure SAML Identity Provider (IdP)
- Create and synchronize custom profile attributes
- Configure profile mappings
- Automate user provisioning
- Automate user profile updates
- Automate user deprovisioning
- Validate successful synchronization between organizations

---

# Technologies Used

- Okta Workforce Identity Cloud
- Okta Org2Org
- SCIM Provisioning
- SAML 2.0
- Okta Profile Editor
- Okta Identity Providers
- Universal Directory
- API Token Authentication
- Attribute Mapping
- User Lifecycle Management

---

# IAM Skills Demonstrated

- Identity Lifecycle Management
- User Provisioning
- User Deprovisioning
- Attribute Mapping
- Identity Federation
- SCIM Provisioning
- SAML Configuration
- Profile Management
- User Assignment
- API Integration
- Identity Synchronization
- Access Management
- Identity Governance Fundamentals

---

# Architecture

```
Source Okta Organization
        │
        │
        ▼
Org2Org Application
        │
        │
SCIM Provisioning
        │
        ▼
Destination Okta Organization

SAML Identity Provider

Profile Mappings

Custom Attributes

Automatic Provisioning

Automatic Updates

Automatic Deprovisioning
```

---

# Lab Walkthrough

## Screenshots

### Step 1 - Configure the Org2Org Application
![Step 1](screenshots/sm_1.png)

### Step 2 - Create API Token
![Step 2](screenshots/sm_2.png)
![Step 3](screenshots/sm_3.png)
![Step 4](screenshots/sm_4.png)
![Step 5](screenshots/sm_5.png)
![Step 6](screenshots/sm_6.png)

### Step 3 - Add the Org2Org Application
![Step 7](screenshots/sm_7.png)
![Step 8](screenshots/sm_8.png)
![Step 9](screenshots/sm_9.png)
![Step 10](screenshots/sm_10.png)

### Step 4 - Configure the SAML Identity Provider
![Step 11](screenshots/sm_11.png)
![Step 12](screenshots/sm_12.1.png)
![Step 13](screenshots/sm_12.2.png)
![Step 14](screenshots/sm_12.3.png)
![Step 15](screenshots/sm_12.4.png)
![Step 16](screenshots/sm_12.5.png)
![Step 17](screenshots/sm_12.6.png)

### Step 5 - Configure API Provisioning
![Step 18](screenshots/sm_13.png)
![Step 19](screenshots/sm_14.png)
![Step 20](screenshots/sm_15.png)
![Step 21](screenshots/sm-16.png)

### Step 6 - Enable Provisioning Features
![Step 22](screenshots/sm_17.png)
![Step 23](screenshots/sm_18.png)
![Step 24](screenshots/sm_19.png)
![Step 25](screenshots/sm_20.png)

### Step 7 - Create the Custom Attribute
![Step 26](screenshots/sm_21.png)
![Step 27](screenshots/sm_22.png)
![Step 28](screenshots/sm_23.png)

### Step 8 - Configure Profile Editor
![Step 29](screenshots/sm_24.png)
![Step 30](screenshots/sm_25.png)
![Step 31](screenshots/sm_26.png)
![Step 32](screenshots/sm_27.png)

### Step 9 - Configure Profile Mapping
![Step 33](screenshots/sm_28.png)
![Step 34](screenshots/sm_29.png)
![Step 35](screenshots/sm_30.png)
![Step 36](screenshots/sm_31.png)

### Step 10 - Force Sync and Verify
![Step 37](screenshots/sm_32.png)
![Step 38](screenshots/sm_33.png)
![Step 39](screenshots/sm_34.png)
![Step 40](screenshots/sm_35.png)
![Step 41](screenshots/sm_36.png)
Successfully demonstrated:

- Enterprise identity federation
- SCIM provisioning
- Automated account creation
- Automated profile synchronization
- Custom attribute synchronization
- API integration
- Identity lifecycle automation
- Automatic deprovisioning
- SAML identity federation
- Profile mapping
- Universal Directory customization

---

# Key IAM Concepts

- Identity Lifecycle Management
- User Provisioning
- User Deprovisioning
- Attribute Mapping
- SCIM
- SAML 2.0
- Identity Federation
- Universal Directory
- Profile Editor
- API Integration
- User Assignment
- Automated Provisioning
- Automated Deactivation
- Access Management
- Identity Governance

---

# Lessons Learned

This project reinforced the importance of identity lifecycle automation within enterprise IAM environments. By combining SCIM provisioning, SAML federation, and custom attribute mapping, users can be automatically created, updated, synchronized, and deactivated across connected identity systems while maintaining consistent profile data.
