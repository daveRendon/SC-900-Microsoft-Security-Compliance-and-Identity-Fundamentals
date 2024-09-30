<!---
---
Demo:
    Title: 'Explore the eDiscovery'
    Learning Path/Module/Unit: 'Learning Path: Describe the capabilities of the Microsoft Priva and Microsoft Purview; Module 3: Describe the data compliance solutions of Microsoft Purview; Unit 2:  Describe eDiscovery'
---
--->

# Demo: Explore eDiscovery (Standard)

This demo maps to the following Learn content:

- Learning Path: Describe the capabilities of the Microsoft Priva and Microsoft Purview
- Module: Describe the data compliance solutions of Microsoft Purview
- Unit:  Describe eDiscovery

## Demo scenario

In this demo you'll do a walk-through of the steps required for setting up eDiscovery, including setting up role permissions, creating an eDiscovery case, creating an eDiscovery hold and creating a search query.  NOTE: In the Microsoft Purview portal updates to the user interface are rolling out, gradually. Some lab/demo tenants may not yet show the newest UI, so all lab steps are shown using the Classic eDiscovery UI.

### Demo Part 1

To access eDiscovery (Standard) or be added as a member of an eDiscovery case, a user must be assigned the appropriate permissions. In this part of the demo, you as the global admin, will walk through the process of adding specific users as members of the eDiscovery Manager role group.

1. Open the browser tab for **Microsoft Purview**. If you previously closed it, open a browser tab and in the address bar, enter **https://purview.microsoft.com**. To access the new Microsoft Purview portal, select the box next to where it says, **I agree to the terms of data flow disclosure and Privacy Statements**, then select **Get started**.  
1. From the left navigation panel, select **Settings**.
1. From the navigation panel that opens, select **Roles and scoped** to expand the option, then select **Role groups**.
1. In the search box on the right side of the screen, search on the term **eDiscovery**.  Select **eDiscovery Manager**.
    1. Select **Edit**.
    1. Select **Choose users**.
    1. Search for MOD Administrator, select the box next to **MOD Administrator** then select the **Select** button on the bottom of the page.
    1. Select **Next** then select **Save**, then finally select **Done**.

1. Keep this browser tab open.

### Demo Part 2

In this part you will create a case to start using eDiscovery (Standard).

1. From the left navigation panel, select **Solutions**, select **eDiscovery** then select **Standard cases**.

1. From the top of the eDiscovery (Standard) page, select **+ Create a case**.

1. In the New case window, enter a Case name, **SC900 Test Case** then select the **Save** at the bottom of the page.

1. The case should now appear on the list.

1. As the creator of the case and because you have eDiscovery Administrator privileges, you can begin to work with it.  

1. Keep this browser tab open.

### Demo Part 3

Now that you've created an eDiscovery (Standard) case, you can begin to work with the case.  In this part, you'll create an eDiscovery hold for the case for you created.  Specifically, you'll create a hold for the exchange mailbox belonging to Adele Vance.

1. From the eDiscovery (Standard) page, select the case you created - **SC900 Test Case**.

1. From the Home page of the case, select the **Hold** tab then select **+Create**.

1. In the name field, enter **Test hold** then select **Next**.

1. In the Choose locations page, select toggle switch next to **Exchange mailboxes** to set the status to **On**.  

1. Now select **Choose users, groups, or teams**.  In the search box, enter **Adele** then press enter on your keyboard. From the search results select **Adele Vance**, then select **Done**.

1. From the Choose locations page, select **Next**.  For expediency with the demo, no other locations will be included in this hold.

1. The Query conditions page enables you to create a hold, based on specific Keywords or Conditions that are satisfied, select **+ Add condition** to view the available options.  Select **Next**. Without any conditions, the hold will preserve all content in the specified location.

1. Review your settings and select **Submit**, it may take a minute, then select **Done**.  The Test hold should appear on the list.  If you don't immediately see it, select **Refresh**

1. Keep this browser tab open.

### Demo Part 4

With a hold in place, you'll create a search query.  Once your search is complete, the eDiscovery supports actions, such as exporting and downloading the results for future investigation.   Note:  Searches associated with an eDiscovery (Standard) case are not listed on the Content search page in the Microsoft Purview compliance portal. These searches are listed only on the Searches page of the associated eDiscovery (Standard) case.

1. From the SC900 Test Case page, select  **Searches**.

1. From the Search page, select **+ New Search**.

1. In the Name field, enter **Test Hold – Sales Search**, then select **Next** from the bottom of the page.

1. In the Choose locations page, select **locations on hold** and deselect **Add App Content for On-Premises users**, as your lab environment has no on-premises  users, then select **Next**.

1. The Query conditions page enables you to create a search, based on specific Keywords or Conditions that are satisfied, In the keyword field enter **Sales** select **Next**.

1. Review your settings and select **Submit**, it may take a minute, then select **Done**.  The search should appear on the list.  If you don't immediately see it, select **Refresh**

1. From the Searches window, select the search you created, **Test Hold - Sales Search**.  A window that opens with the Summary tab selected.  Once the search is complete the status will indicate that the search is completed.  You'll see a Search statistics tab (if you don't see the Search statistics tab, the search may still be running and may take a few minutes to complete).  Select the **Search statistics** tab and select the down-arrow next to Search content.  You can also view more information for the Condition report and Top locations.  

1. From the bottom of the page, select **Actions**.  Note the available options that include export options. Select **Close**.

1. Close all the open browser tabs.

### Review

In this demo, you went through the steps required to get started with eDiscovery (Standard), including setting up the role permissions for eDiscovery and creating an eDiscovery case.  With the case, created you went through elements of the eDiscovery (Standard) workflow by creating an eDiscovery hold and creating a search query.
