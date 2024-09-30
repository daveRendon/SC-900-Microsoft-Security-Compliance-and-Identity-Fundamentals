---
lab:
    title: 'Microsoft Entra Conditional Access'
    module: 'Describe the access management capabilities of Microsoft Entra'
---

# Lab: Microsoft Entra Conditional Access

This lab maps to the following Learn content:

- Learning Path: Describe the capabilities of Microsoft Entra
- Module: Describe access management capabilities of Microsoft Entra
- Unit: Describe Conditional Access

## Lab scenario

In this lab, you'll explore conditional access MFA, from the perspective of an admin and a user.  As the admin, you will create a policy that will require a user to go through multi-factor authentication when accessing any of the Microsoft Admin portals.  From a user perspective, you'll see the impact of the conditional access policy, including the process to register for MFA.

**Estimated Time**: 30 minutes

### Task 1

In this task you, as the admin, will reset the password for the user Debra Berger.  This step is needed so you can initially sign in as the user in subsequent tasks.

1. Open Microsoft Edge.  In the address bar, enter **https://entra.microsoft.com**, and sign in with your admin credentials.
    1. In the Sign-in window, enter **admin@WWLxZZZZZZ.onmicrosoft.com** (where ZZZZZZ is your unique tenant ID provided by your lab hosting provider) then select **Next**.
    1. Enter the admin password that should be provided by your lab hosting provider. Select **Sign in**.
    1. When prompted to stay signed- in, select **Yes**.

1. From the left navigation pane, expand **Identity**, expand **Users**, then select **All users**.

1. Select **Debra Berger** from the list of users.

1. Select **Reset password** from the top of the page. Since you haven't previously signed in as Debra Berger, you don’t know her password, and will need to reset the password.

1. When the password reset window opens, select **Reset Password**.  IMPORTANT, make a note of the new password, as you'll need it in a subsequent task, to be able to sign in as the user.

1. Close the password reset window by selecting the **X** at the top right corner of the page, then close out of the Debra Berger window by selecting the **X** at the top right corner of the page.

1. From the left navigation panel, select **Home** to return to the Microsoft Entra admin center.

1. Keep this window open.

### Task 2

In this task, you'll go through the process of creating a conditional access policy in Microsoft Entra ID.

1. Open the browser tab to the home page of the Microsoft Entra admin center.   If you previously closed the browser tab, open Microsoft Edge and in the address bar enter **https://entra.microsoft.com** and sign in with the Microsoft 365 admin credentials provided by the ALH.

1. From the left navigation pane, expand **Protection** then select **Conditional Access**.

1. The Conditional access overview page is displayed.  Here you will see tiles showing the Policy summary and general alerts.  From the left navigation panel, select **Policies**.

1. From the left navigation panel, select **Policies**. Any existing Conditional Access Policies are listed here. Select **+ New policy**.

1. In the Name field, enter **MFA Test Policy**.

1. Under Users, select **0 users and groups selected**.

1. You'll now see the option to Include or Exclude users or groups.  Make sure **Include** is selected (underlined).

1. Select the option for **Select users and groups** and select **Users and groups**.  The window to Select users and groups opens.  

1. In the Search bar, enter **Debra**.  Select **Debra Berger** from beneath the search bar, then press the **Select** button on the bottom of the page.  Note, a common practice is to assign the policy to users in a group.  For the purpose expediency with this lab, we'll assign the policy to a specific user.

1. Under Target resources, select **No target resources selected**.

1. In the field underneath where it says **Select what this policy applies to**, select the down-arrow and note the available options.  Keep the default setting, **Cloud apps**.  Make sure the **Include** tab is underlined.  Select **Select apps**, then underneath where it says **Select**, select **None**.  The window to Select Cloud apps opens.

1. Select **Microsoft Admin Portals**, then press **Select** at the bottom of the page.  Notice the warning.  

1. Under Network, select **Any network or location**.  Review the options but do not select any options.

1. Under Conditions, select **0 conditions selected**.  Notice the different options you can configure.  Through the policy, you can control user access based on signals from conditions including: user risk, sign-in risk, device platform, location, client apps, or filter for devices.  Explore these configurable options, but do not set any conditions.

1. Now you'll set the access controls.  Under Grant, select **0 controls selected**.

1. The Grant window opens.  Ensure **Grant access** is selected and then select **Require multifactor authentication**. Scroll down a bit on the right window and under the section For multiple controls, leave the default **Require all the selected controls**.  Press **Select** at the bottom of the page.

1. At the bottom of the page, Under Enable policy, select **On**, then select **Create**.

1. From the left navigation pane select **Policies**. The MFA Pilot policy should appear in the list of conditional access policies (if needed, select the **Refresh icon** in the command bar at the top of the page).

1. Sign out by selecting on the user icon next to the email address on the top right corner of the screen and selecting **Sign out**. Then the close all the browser windows

### Task 3

In this task you'll see the impact of the conditional access policy, from the perspective of the user, Debra Berger. You'll start first by signing-in to an application that is not included in the conditional access policy (the Microsoft 365 portal at https://login.microsoftonline.com).  Then you'll repeat the process for an application that is included in the conditional access policy (the Azure portal at https://portal.azure.com).  Recall that the policy requires the user to go through MFA when accessing any of the Microsoft Admin Portals, including the Azure portal.  To use MFA, the user must first register the authentication method that will be used for MFA, for example a code sent to a mobile device or an authenticator application.

1. Open Microsoft Edge.  In the address bar, enter **https://login.microsoftonline.com**.
    1. Sign in as **DebraB@WWLxZZZZZZ.onmicrosoft.com** (where ZZZZZZ is your unique tenant ID provided by your lab hosting provider) then select **Next**.
    1. Enter the password you noted in the earlier task. Select **Sign in**.
    1. Since the password provided when you, as the admin, reset the password is temporary you need to update your password (this is not part of the MFA policy). Enter the current password, then enter a new password and then confirm the new password.  Make note of the new password as you will need it to complete the task.
    1. When prompted to stay signed- in, select **Yes**.  You should be successfully logged in to your Microsoft 365 account. MFA was not required for this application as it is not part of the policy.

1. Now you'll attempt to sign in to an application that meets the criteria for MFA. Open a new browser tab and enter **https://portal.azure.com**.

1. You'll see a window indicating, More information required.  Select **Next**.  Note, this will initiate the MFA registration process, as this is the first time you're accessing the cloud app that that was identified in the conditional access policy.  This registration process is required only once.   An alternative to having the user go through the registration process is to have the admin configure the authentication method to use.

1. In the Keep your account secure window, you have the option to select the method to use for MFA.  Microsoft Authenticator is one option. For expediency in this lab exercise, you'll choose a different method.  Select **I want to setup a different method**.  From the Chose a different method pop-up window, select the **drop-down arrow** and select **Phone** then select **Confirm**.

1. The window that appears and the steps that follow are for the Microsoft Authenticator app method. .
    1. If you already have the Microsoft Authenticator app installed on your mobile device select **Next**. Otherwise, select **Download now** and follow the steps.
    1. You'll begin to setup your account.  Select **Next**.
    1. Using the Microsoft Authenticator app on your mobile device, select the **+** to add an account and select **Work or school account**.
    1. Select the option to **Scan the QR code**, then using your mobile device, scan the QR code on your PC screen .
    1. Using the Microsoft Authenticator app on your mobile device, scan the QR code.
    1. Follow the steps on your PC and mobile device, then select **Next**.
    1. Once you've setup your security info, you'll see a Success window.  Select **Done**.

1. You should now be able to access the Azure portal.  The Azure portal is a Microsoft Admin portal and therefore requires multi-factor authentication, per the conditional access policy that was created.  
    1. If you get a message indicating that your sign-in timed out you, enter the password and select **Sign in**.
    1. You'll see a window that requires you to approve the sign in request.  Note the number on your PC and follow the instructions on the Microsoft Authenticator app.
    1. If you're prompted to stay signed in, select **No**.

1. Sign out by selecting on the user icon next to the email address on the top right corner of the screen and selecting sign out. Then the close all the browser windows.

### Review

In this lab, you went through the process of setting up a conditional access policy that requires users to go through MFA when they access any Microsoft Admin portal.  Then, as a user you went through the registration process for MFA and saw the impact of the conditional access policy that required you to use MFA when accessing the Azure portal.
