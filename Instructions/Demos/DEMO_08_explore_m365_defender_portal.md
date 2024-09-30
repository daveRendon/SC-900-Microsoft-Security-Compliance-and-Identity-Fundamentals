<!---
---
Demo:
    Title: 'The Microsoft Defender portal'
    Module: 'Learning Path: Describe the capabilities of Microsoft security solutions; Module 4: Describe the threat protection capabilities of Microsoft Defender XDR; Unit 7: Describe the Microsoft Defender portal'
---
--->

# Demo: The Microsoft Defender portal

This demo maps to the following Learn content:

- Learning Path: Describe the capabilities of Microsoft security solutions
- Module: Describe the threat protection capabilities of Microsoft Defender XDR
- Unit: Describe the Microsoft Defender portal

## Demo scenario

In this demo, you'll show the Microsoft Defender portal by walking through the content displayed on the landing page. You'll also walk through the options on the navigation panel that provide quick access to functionality that is part of Microsoft’s Extended Detection and Response (XDR) solution: Microsoft Defender for Endpoints, and Microsoft Defender for Office 365 (email and collaboration).  Lastly you'll also show how Microsoft Secure Score can help an organization improve its security posture.

### Demo Part 1

Explore the Microsoft Defender landing page.

1. Open the browser tab for the Microsoft Defender home page.  If you previously closed the browser, open Microsoft Edge. In the address bar, enter **https://admin.microsoft.com** and sign in with the admin credentials for the Microsoft 365 tenant provided by your authorized lab hoster (ALH), to access the Microsoft 365 admin center. From the left navigation pane of the Microsoft 365 admin center, select **Show all** then select **Security**.  A new browser page opens to the welcome page of the Microsoft Defender portal.  

1. The home page of the Microsoft Defender portal shows many of the common cards that security teams need. The composition of cards and data is dependent on the user role. Scroll through the page to view the default set of cards for your role as global admin.

1. The cards displayed can be customized to your preference.  Select **+ Add cards**. A Window opens that displays any cards that are available to add to your home page.  You may already have all cards displayed in which case you will see the note, "You already have all the cards on your home page." Close the window by select the **X** on top-right corner of the window.

1. Selecting the ellipses on the top-right of any card will provide the option to remove the card from the landing page.  

1. You can also move the cards around. Hover your mouse cursor over the title bar of any card,  when you'll get a cross shaped cursor select the card and move it to your desired location.  

1. Some cards have buttons on the bottom of the card that are selectable. The title of some cards serve as a link to the page for that topic.  For example, if you select the title of the Microsoft Secure Score card, it will take you to the Microsoft Secure Score page.  You'll explore more about Microsoft Secure Score in a subsequent section of this demo.

1. Keep the browser window open.

### Demo Part 2

In this part of the demo, you'll explore some of the options available from the left navigation panel of the Defender portal.  Through the Microsoft Defender portal, Microsoft delivers on the promise of a unified security operations platform. The Microsoft Defender portal combines protection, detection, investigation, and response to threats across your entire organization and all its components, in a central place. It includes quick access to the Microsoft Defender XDR solutions, including Microsoft Defender for Endpoint, Defender for Office for 365, Microsoft Defender for Cloud Apps, and more.  Explore these options by selecting some of the links.   To return to the home page of the Microsoft Defender portal, select **Home** on the left navigation panel.

**NOTE: the intent is to walk through some of the options on the navigation panel, it is not intended as a full demo of all the options**.

1. **Exposure management** - The options listed provide a unified view of security posture across company assets and workloads.
    1. **Attack surface** - You can view the Attack Surface Map for your organization. Attack paths automatically generates attack paths based on the data collected across assets and workloads. It simulates attack scenarios, and identifies vulnerabilities and weaknesses that an attacker could exploit.
    1. **Security insights** - Exposure insights in Microsoft Security Exposure Management continuously aggregate security posture data and insights across workloads and resources, into a single pipeline.
    1. **Secure score** - Secure Score provides a breakdown of the score, the improvement actions that can boost the organization's score, and how well the organization's Secure Score compares to other similar organizations.
    1. **Data connectors** - Here connect data sources for a richer, more centralized exposure management experience.
1. **Investigation & response** - From here you'll see several options:
    1. **Incidents & alerts** - From here you view the incidents or individual alerts from the different Defender XDR solutions (Defender for Identity, Defender for Cloud apps, Defender for Office 365, and Defender for Identity) and other Microsoft solutions including Microsoft Sentinel, Microsoft Defender for Cloud, Microsoft Entra, and Microsoft Purview.
    1. **Hunting** - From here you can build custom detection rules and hunt for specific threats in your environment.
    1. **Actions and submissions** - The unified Action center brings together remediation actions across Microsoft Defender for Endpoint and Microsoft Defender for Office 365. It lists pending and completed remediation actions for your devices, email & collaboration content, and identities in one location. In Microsoft 365 organizations with Exchange Online mailboxes, admins can use the Submissions page in the Microsoft Defender portal to submit messages, URLs, and attachments to Microsoft for analysis.
    1. **Partner catalog** - The partner catalog lists supported technology partners and professional services that can help your organization enhance the detection, investigation, and threat intelligence capabilities of the platform.
1. **Threat Intelligence** - From the Threat Intelligence tab, users access Microsoft Defender Threat Intelligence and the capabilities the solution supports, including Threat analytics, intel profiles, intel explorer, and intel projects.
1. **Assets** - The Assets tab allows you to view and manage your organization's inventory of protected and discovered assets (devices and identities).
1. **Microsoft Sentinel** - Some Microsoft Sentinel capabilities are available in the Microsoft Sentinel section of the Defender portal.  This requires setting up the integration through the Settings page.
1. **Identities** - The Identities node maps to functionality associated with Microsoft Defender for Identity. The Dashboard provides critical insights and real time data about identity threat detection and response (ITDR). The health Issues page lists any current health issues for your Defender for Identity deployment and sensors, alerting you to any problems in your Defender for Identity deployment. The tools page lists additional information to help manage your Microsoft Defender for Identity environment.
1. **Endpoints** - Endpoints node on the left navigation panel of the Microsoft Defender portal maps to functionality associated with Microsoft Defender for Endpoints.
    1. Vulnerability management - Manage vulnerabilities and other risk sources on devices. From here you can access the vulnerability management dashboard, recommendations, remediation, weaknesses, and more.
    1. Partners and API - From here you can select Connected applications and API explorer.
    1. Configuration Management - here you can view the Device configuration management dashboard.  You can also define endpoint policies and track deployment.
1. **Email & collaboration** - This is where you find Microsoft Defender for Office 365 functionality that allows you to track and investigate threats to your users' email, track campaigns, and more.
1. **Cloud apps** -  This is where you find Microsoft Defender for Cloud Apps functionality. Refer to the demo on Microsoft Defender for Cloud apps for more information.
1. **SOC Optimization** - SOC optimization surfaces ways you can optimize your security controls, gaining more value from Microsoft security services as time goes on.
1. **Reports** - Reports are unified in the Microsoft Defender portal. Admins can start with a general security report, and branch into specific reports about endpoints, email & collaboration, cloud apps, infrastructure, and identities. The links here are dynamically generated based upon workload configuration.
1. **Leraning hub** - The learning hub links you Microsoft Learn where you can get access to training courses, tutorials, documentation, and other relevant material.
1. **System** - This includes selections to configure permissions, view service health, and general settings.
    1. Permissions - Here you can assign role permissions for the different Microsoft Defender XDR solutions.
    1. Settings - Here you configure settings for the Defender portal, Defender XDR, solutions that are part of Microsoft Defender XDR, and Microsoft Sentinel.  Explore this at will.
1. **Customize Navigation** - Here you can select to show or hide items in your navigation pane. Other admins will not see your changes.

### Demo Part 3

In this part of the demo, you'll show how Microsoft Secure Score can help an organization improve its security posture.

1. From the from the left navigation panel, expand **Exposure management** then select **Secure Score**.

1. The Microsoft Secure Score page opens to the Overview tab.  Microsoft Secure Score is a measurement of an organization's security posture. Your organization’s secure score is shown as a percentage, along with the number of points you've achieved out of the total possible points and broken down by category. Select **Include**, next to where it says Your secure score. you can choose for the view of your score to include the achievable score, Planned score, and Current license score.

1. The overview page also includes top recommended actions, comparison score, history, and resources.

1. Select **Recommended actions** from the top of the page.  Notice the information available for each item in the table.  

1. Select the first items from the list and review the available information. In the window that opens, note the status options available. Select the **Implementation** tab to view to view information related to implementation. Select the **X** at the top right corner to close this window.

1. Select the **History** tab from the top of the page.  For each activity listed there is a brief statement that provides context.  Select an item from the history table.  On the top-right of the details page, under History, select **X events** (where X is a number).  The action history window opens and provides more information.  Select **Close** on the bottom of the page, then select the **X** on the top-right corner of the details page to return to the History page.

1. From the top of the page, select **Metrics & trends**.  Note the available information.  From the top-right corner of the page, select the **calendar icon**.  You can narrow down the view to a custom date range.  Selecting the **filter icon**, allows you to filter the view by Identity, Devices, and/or apps.  Close the window.

1. From the left navigation panel, select **Home** to the home page for Microsoft Defender.

1. Keep the browser tab open if you plan to continue with the next demo.

### Review

In this demo, you explored the Microsoft Defender portal by walking through the content displayed on the landing page, you explored the options on the navigation panel that provides quick access to functionality that is part of Microsoft Defender XDR.  Lastly you showed how Microsoft Secure Score can help an organization improve its security posture.
