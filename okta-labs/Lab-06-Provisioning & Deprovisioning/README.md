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

### Step 1 - Configure Org2Org Application
![Step 1](images/step1.png)

### Step 2 - Enable API Integration
![Step 2](images/step2.png)

### Step 3 - Enable Provisioning
![Step 3](images/step3.png)

### Step 4 - Open Profile Editor
![Step 4](images/step4.png)

### Step 5 - Create Preferred Name Attribute
![Step 5](images/step5.png)

### Step 6 - Add Attribute to Org2Org Profile
![Step 6](images/step6.png)

### Step 7 - Add Attribute to SAML IdP Profile
![Step 7](images/step7.png)

### Step 8 - Configure Profile Mappings
![Step 8](images/step8.png)

### Step 9 - Force Sync
![Step 9](images/step9.png)

### Step 10 - Assign User
![Step 10](images/step10.png)

### Step 11 - Verify Provisioned User
![Step 11](images/step11.png)

### Step 12 - Verify Preferred Name Sync
![Step 12](images/step12.png)

### Step 13 - Unassign User
![Step 13](images/step13.png)

### Step 14 - Verify User Deactivation
![Step 14](images/step14.png)

# Results

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
