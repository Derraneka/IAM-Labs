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

---

## Step 1 - Configure the Org2Org Application

The Org2Org application was configured to establish trust between two Okta organizations.

**Screenshot**

```
Insert Screenshot 1
```

---

## Step 2 - Enable API Integration

API Integration was enabled using an Okta API Security Token.

This allows SCIM provisioning features such as:

- Create Users
- Update User Attributes
- Deactivate Users

**Screenshot**

```
Insert Screenshot 2
```

---

## Step 3 - Enable Provisioning Features

Provisioning settings were configured to automate identity lifecycle operations.

Enabled:

- Create Users
- Update User Attributes
- Deactivate Users

Password synchronization was intentionally left disabled.

**Screenshot**

```
Insert Screenshot 3
```

---

## Step 4 - Open Profile Editor

The Okta Universal Directory Profile Editor was opened to extend the user schema.

**Screenshot**

```
Insert Screenshot 4
```

---

## Step 5 - Create a Custom User Attribute

A custom attribute named:

```
preferredname
```

was added to the Okta User Profile.

Attribute Details

| Property | Value |
|----------|-------|
| Display Name | Preferred Name |
| Variable Name | preferredname |
| Data Type | String |

**Screenshot**

```
Insert Screenshot 5
```

---

## Step 6 - Add the Attribute to the Org2Org Application Profile

The custom attribute was added to the Org2Org application profile so it could participate in provisioning.

**Screenshot**

```
Insert Screenshot 6
```

---

## Step 7 - Configure the Identity Provider Profile

The SAML Identity Provider profile schema was updated to include the same custom attribute.

This ensures the attribute exists across both identity stores.

**Screenshot**

```
Insert Screenshot 7
```

---

## Step 8 - Configure Profile Mappings

Profile mappings were updated to synchronize user attributes from the Okta User Profile to the Identity Provider.

Mapped attributes included:

- First Name
- Last Name
- Email
- Mobile Phone
- Department
- Title
- Preferred Name

Mappings were configured to apply during:

- User Creation
- User Updates

**Screenshot**

```
Insert Screenshot 8
```

---

## Step 9 - Force Synchronization

A Force Sync operation was executed to immediately push updated mappings to the destination organization.

**Screenshot**

```
Insert Screenshot 9
```

---

## Step 10 - Assign a User

A user was assigned to the Org2Org application.

Assignment automatically triggered SCIM provisioning.

**Screenshot**

```
Insert Screenshot 10
```

---

## Step 11 - Verify User Creation

The destination organization was inspected to verify the account had been successfully provisioned.

Verification included:

- User Account
- Email Address
- Active Status

**Screenshot**

```
Insert Screenshot 11
```

---

## Step 12 - Verify Attribute Synchronization

The destination user profile was reviewed.

The following synchronized successfully:

- Department
- Title
- Preferred Name

The custom **preferredname** attribute correctly transferred between organizations.

**Screenshot**

## Step 1 - Configure the Org2Org Application

The Org2Org application was created to establish trust between two Okta organizations.

![Step 1 - Org2Org Application](images/step1-org2org-application.png)

---

## Step 2 - Enable API Integration

API Integration was enabled using an Okta API Token, allowing SCIM provisioning capabilities between organizations.

![Step 2 - API Integration](images/step2-api-integration.png)

---

## Step 3 - Enable Provisioning Features

Provisioning settings were configured to automatically:

- Create Users
- Update User Attributes
- Deactivate Users

![Step 3 - Provisioning Settings](images/step3-provisioning-settings.png)

---

## Step 4 - Open the Profile Editor

The Okta Universal Directory Profile Editor was used to extend the user schema.

![Step 4 - Profile Editor](images/step4-profile-editor.png)

---

## Step 5 - Create a Custom User Attribute

A custom attribute named **preferredname** was added to the Okta User profile.

Attribute Details

| Property | Value |
|----------|-------|
| Display Name | Preferred Name |
| Variable Name | preferredname |
| Data Type | String |

![Step 5 - Add Custom Attribute](images/step5-add-custom-attribute.png)

---

## Step 6 - Add the Attribute to the Org2Org Profile

The custom attribute was added to the Org2Org application profile so it could be provisioned to the destination organization.

![Step 6 - Org2Org Profile Attribute](images/step6-org2org-profile.png)

---

## Step 7 - Configure the Identity Provider Profile

The SAML Identity Provider profile schema was updated to include the **preferredname** attribute.

![Step 7 - Identity Provider Attribute](images/step7-idp-profile.png)

---

## Step 8 - Configure Profile Mappings

Profile mappings were configured so the following attributes synchronize automatically:

- First Name
- Last Name
- Email
- Mobile Phone
- Department
- Title
- Preferred Name

Mappings were configured to apply during user creation and updates.

![Step 8 - Profile Mapping](images/step8-profile-mapping.png)

---

## Step 9 - Force Synchronization

A Force Sync operation was performed to immediately push the updated profile mappings to the destination organization.

![Step 9 - Force Sync](images/step9-force-sync.png)

---

## Step 10 - Assign a User

A user was assigned to the Org2Org application, triggering automatic SCIM provisioning.

![Step 10 - User Assignment](images/step10-user-assignment.png)

---

## Step 11 - Verify User Creation

The destination Okta organization confirmed that the user account was successfully provisioned.

Verification included:

- User account
- Email address
- Active status

![Step 11 - Provisioned User](images/step11-user-created.png)

---

## Step 12 - Verify Attribute Synchronization

The destination user's profile confirmed that custom and standard attributes synchronized successfully.

Verified attributes included:

- Department
- Title
- Preferred Name

![Step 12 - Attribute Sync](images/step12-attribute-sync.png)

---

## Step 13 - Deprovision the User

The user was unassigned from the Org2Org application, automatically triggering SCIM deprovisioning.

![Step 13 - User Unassignment](images/step13-unassign-user.png)

---

## Step 14 - Verify Automatic Deactivation

The destination organization confirmed that the user's account status changed from **Active** to **Deactivated**, demonstrating successful automated lifecycle management.

![Step 14 - User Deactivated](images/step14-user-deactivated.png)

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
