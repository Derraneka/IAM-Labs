# Lab 1 — Create Users in Okta

## Objective

Create and manage user accounts in Okta.

## Scenario

A new employee needs access to Okta. Create the user account, update the user profile, and verify the lifecycle activity in the System Log.

---

## Create a user account

### Step 1

From the Admin Console, go to **Directory > People**.

### Step 2

Click **Add Person** and enter the user details.

![Add Person](./images/add-person.png)

### Step 3

Complete the required profile fields.

![User Details](./images/user-details.png)

### Step 4

Click **Save** and confirm the user appears in the People list.

![User Created](./images/user-created.png)

> Note: In a real-world environment, activation emails are usually sent to users. Setting a password manually is mostly used for testing or lab accounts.

---

## Modify the user profile

### Step 5

In **Directory > People**, select the user account.

### Step 6

Open the **Profile** tab and edit the user attributes.

![Edit Profile](./images/edit-profile.png)

### Step 7

Save the changes and verify the updated profile information.

![Updated Profile](./images/updated-profile.png)

---

## View user lifecycle activity

### Step 8

Go to **Reports > System Log**.

### Step 9

Search using this filter:

```eventType sw "user.lifecycle"```

### Step 10

Verify the log shows user lifecycle events such as **Create user**, **Activate user**, or **Update user**.

![System Log](./images/system-log.png)

---

## Skills Practiced

- User account creation
- User profile management
- Okta Admin Console navigation
- User lifecycle monitoring
- System Log filtering
- Identity and Access Management basics

---

## Outcome

Successfully created a user account, modified user profile attributes, and verified lifecycle activity in Okta System Log.
