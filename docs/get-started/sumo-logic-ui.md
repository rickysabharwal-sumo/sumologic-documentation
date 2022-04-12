---
id: sumo-logic-ui
---

# Tour the Sumo Logic UI

Welcome to Sumo Logic introduced you to the process of getting data into Sumo Logic, searching and analyzing your data, then sharing your findings with your colleagues. This page familiarizes you with the Sumo Logic user interface (UI) by showing you how to:

* [Use the Left Navigation Bar](#using-the-left-navigation-bar)
* [Work with tabs](#working-with-tabs)
* [Master everyday tasks](#mastering-everyday-tasks)
* [Become a Sumo Pro user](#become-a-sumo-pro-user)

## Using the Left Navigation Bar

You land on the Sumo Logic Home page when you first log in. The **Left Nav Bar** menu bar is a one-stop location where you can:

* [Access dashboard and searches](#access-dashboards-and-searches)
* [Search and switch browsing modes](#search-and-switch-browsing-modes)
* [Hide and show the Left Nav Bar](#hide-and-show-the-left-nav-bar)
* [Access Apps, Admin features, and Help](#access-apps-admin-features-and-help)

### Access dashboards and searches

The **Left Nav Bar** provides easy access to libraries, personal collections of dashboards, searches, and folders. Click the icons at the top of the Left Nav Bar (left to right ) to view:

* **Recent** dashboards and searches,
* a list of your **Favorites** (dashboards and searches),
* your **Personal** library of dashboards and searches, and
* a **Library** of shared dashboards and searches (within your organization) respectively.

![TUI_Left_Nav.png](/img/get-started/ui/TUI_Left_Nav.png)

### Search and switch browsing modes

The top of the **Left Nav Bar** is where you can search for content and
users and easily switch browsing modes. 

* Searching—Enter text in the **Search** field to quickly find apps, dashboards, searches, and users. 
* Switching browsing modes—Click the **Details** icon and make a selection from the drop-down menu.

![TUI_Search_Details.png](/img/get-started/ui/TUI_Search_Details.png)

### Hide and show the Left Nav Bar

You can easily hide the **Left Nav Bar** to enlarge the working area. Then, just as easily show it again.

* To hide the Left Nav Bar, click the **Arrow** in the top right corner.

    ![TUI_NavBar_Hide.png](/img/get-started/ui/TUI_NavBar_Hide.png)

* To show a hidden Left Nave Bar, click the **Menu** icon.

    ![TUI_NavBar_Show.png](/img/get-started/ui/TUI_NavBar_Show.png)

### Access Apps, Admin features, and Help

In the lower section of the Left Nav Bar, you can access the [App Catalog](library/sumo-logic-apps.md), [Manage Data and Administration] (../Manage.md "Manage") features, and [get help](#get-help-docs-community-and-more). 

![TUI_App-Admin-Help.png](/img/get-started/ui/TUI_App-Admin-Help.png)

## Working with tabs

Every page you select opens in a new tab, and the tabs are shown at the top of the UI. You can have up to 50 tabs open at one time. Each of the following selections opens a new tab:

* Saved search 
* Dashboard
* New log search, metrics visualization or Live Tail session
* App catalog 
* Manage pages 
* Account page 

![WTS_UI_Tabs.png](/img/get-started/ui/WTS_UI_Tabs.png)

### Rename or close a tab

You can customize tabs by renaming them, then close them when they are no longer relevant.

To rename or close a tab, do the following:

1. To rename a tab, double-click the name field, enter the new name, and press **Return**.

    ![WTS_UI_Tab-rename.png](/img/get-started/ui/WTS_UI_Tab-rename.png)

1. To close a tab, hover the cursor over the tab and click the X icon on the right.

    ![WTS_UI_Tab-delete.png](/img/get-started/ui/WTS_UI_Tab-delete.png)

### Customize your environment with tab options

Log Search, Metrics, and Live Tail tabs have additional options you can use to customize your environment. The tabs even stay open when you sign out and sign back in again, so you can start where you left off. Clicking any of the following icons opens a tabbed window.

![WTS_UI_LogSearch-Metrics-LiveTail.png](/img/get-started/ui/WTS_UI_LogSearch-Metrics-LiveTail.png)

To access additional Log Search, Metrics, and Live Tail options, do the following:

1. Hover the cursor over the tab **Details** icon.

    ![WTS_Tab-options-details.png](/img/get-started/ui/WTS_Tab-options-details.png)

1. Select the tab and choose an option from the drop-down menu.

    ![tab options.png](/img/get-started/ui/tab-options.png)

1. Use the left (**\<**) and right (**\\>**) arrows at each end of the Tab menu bar to move back and forth through the tabs.

The following table lists the options available for the Search, Metrics, and Live Tail tabs.

| Option | Search tab  | Metrics tab  | Live Tail tab |
|--|--|--|--|
| Pin | ![check](/img/reuse/check.png) | — | — |
| Open a New Browser Tab | — | — | ![check](/img/reuse/check.png)  |
| Rename | ![check](/img/reuse/check.png) | ![check](/img/reuse/check.png) | ![check](/img/reuse/check.png)  |
| Duplicate | ![check](/img/reuse/check.png) | ![check](/img/reuse/check.png) | ![check](/img/reuse/check.png)  |
| Close | ![check](/img/reuse/check.png) | ![check](/img/reuse/check.png) |  ![check](/img/reuse/check.png) |
| Close Other Tabs | ![check](/img/reuse/check.png) | ![check](/img/reuse/check.png) | ![check](/img/reuse/check.png)  |
| Close All Tabs | ![check](/img/reuse/check.png) | ![check](/img/reuse/check.png) | ![check](/img/reuse/check.png)  |

## Mastering everyday tasks

This section provides information on how to perform basic everyday tasks using the Sumo Logic UI.

**All users:**

* [Launch log searches, metrics visualizations, and Live Tail sessions](#launch-searches-metrics-visualizations-and-live-tail-sessions)
* [View recent dashboards and searches](#view-recent-dashboards-and-searches)
* [View Favorites and add dashboards and searches to the list](#view-favorites-and-add-dashboards-and-searches-to-the-list)
* [Share a dashboard, search, or folder](#share-a-dashboard-search-or-folder)
* [View content that is shared with you](#view-content-that-is-shared-with-you)
* [Pin and manage searches](#pin-and-manage-searches)
* [Manage your personal account preferences](#manage-your-personal-account-preferences)
* [Get help: docs, community, and more](#get-help-docs-community-and-more)

**Sumo Logic Administrators:**

* [Admin: Manage data collection, data settings, and alerts](#admin-manage-data-collection-data-settings-and-alerts)
* [Admin: Manage accounts, users, and security](#admin-manage-accounts-users-and-security)

### Launch searches, metrics visualizations, and Live Tail sessions 

This section shows you how to get started working with logs and metrics. The links provided direct you to more in-depth information.

To launch a search, metrics visualization, or live tail session, do the following:

1. Go to the Sumo **Home** page.
1. Do one of the following:

   * Click **+New** in the Tabs menu and choose an option from the drop-down menu. 
   * Click one of the following Home page icons:

     * [Log Search]  (../05Search/Get-Started-with-Search/Search-Basics.md "Search Basics"). Open the Search page to search logs.
     * [Metrics] (../Metrics.md "Metrics"). Open the Metrics page to create a metrics visualization.
     * [Live Tail] (../05Search/Live-Tail.md "Live Tail"). View a real-time live feed of log events associated with a Source or Collector.

    ![WTS_UI_Search-Metrics-LiveTail.png](/img/get-started/ui/WTS_UI_Search-Metrics-LiveTail.png)

### View recent dashboards and searches 

You see the Home landing page when you first log in to Sumo Logic. The Home page provides an at-a-glance view of the following:

* recently opened dashboards
* recently run searches
* recommended dashboards 
* pinned searches

Click the **Home** icon at the far left of the Tab menu bar to return to the Home page at any time.

![WTS_UI_Home_landing-page.png](/img/get-started/ui/WTS_UI_Home_landing-page.png)

### View Favorites and add dashboards and searches to the list

You can create a list of favorite dashboards and searches that appear in the Left Nav Bar. Your Favorites list makes it easy to access your most frequently used dashboards and searches.

To view Favorites and add to the list, do the following:

1. To view a list of current Favorites, click the **Star** icon at the top of the Left Nav Bar. A list of Favorites is shown below.

    ![WTS_UI_View_list-of-Favorites.png](/img/get-started/ui/WTS_UI_View_list-of-Favorites.png)

1. To add a dashboard to the Favorites list, open the dashboard, select the **Details** icon at the top right of the menu bar and select **Favorite** from the drop-down list. 

    ![WTS_UI_Add-dashboard-to-Favorites.png](/img/get-started/ui/WTS_UI_Add-dashboard-to-Favorites.png)

1. To add a search to the Favorites list, do the following:

   1. [Save the search](../search/get-started-with-search/search-basics/save-search.md) (if not already saved) by clicking **Save As**, then in the Save Item dialog enter a name, description, and select a folder in which to save the search.
   1. Click **Save**.
   1. Click the three-dot icon and click **Favorite** from the provided options. 

![favorite saved search ](/img/get-started/ui/favorite-saved-search.png)

The dashboard and search appear in the Favorites list in the Left Nav Bar.

![WTS_UI_Additions-to-Favorites-list.png](/img/get-started/ui/WTS_UI_Additions-to-Favorites-list.png)

### Share a dashboard, search, or folder

You can share dashboards, searches, and folders with users and roles. You can edit the sharing permissions at any time and share or revoke permissions as needed. You can share content from the following locations:

* **Left Nav Bar.** Recommended when you are familiar with the content and need to quickly share with another user.
* **Library.** Recommended when you need a detailed view of the content, who created it, and when it was last modified.

For walkthrough instructions, go to the [Share Content] (../Manage/Content_Sharing/Share-Content.md "Share Content") page. 

### View content that is shared with you

It's easy to view dashboards, searches, and folders that have been shared with you.

To see content that has been shared with you, do the following:

1.  Click the **Clock** icon at the top of the Left Nav Bar.
2.  Toggle between **Recently Opened By Me** or **Recently Shared With Me**.

![Dash3.png](/img/get-started/ui/Dash3.png)

### Pin and manage searches

After you start a search, you can “pin” it, and it will run in the background for up to 24 hours. If the search does not finish in that time frame, it is paused. You can restart the search at any time. Search results are available for three days.

There is a limit of ten pinned searches per user. Also, queries that use the [save operator](../search/search-query-language/search-operators/save-lookups-classic.md) cannot be pinned.

You must start a search for the Pin option to appear. Once a search is pinned, it cannot be unpinned, but it can be removed from the Pinned Searches tab.

To pin a search, do the following:

1. Open a Search page.
1. Enter a query in the search box and click **Start**.
1. Click the three-dot icon and click **Pin** from the provided options.

    ![pin search](/img/get-started/ui/pin-search.png)

1. A message appears telling you the location of your pinned search in the Library. The Pinned Search takes the name of the Search tab by default.

    ![pinmessage.png](/img/get-started/ui/pinmessage.png)

1. To change the name of a Pinned Search, double-click the Search tab and enter a new name in the name field.

For information on how to manage pinned searches, see the [Pinned Searches](library/search-the-library.md) page.

### Manage your personal account preferences

You can manage your personal account settings from the **Preferences** page. These settings **only apply** to your account. Changes you make to your preferences take effect the next time you sign in, not during the current session.

To manage your personal Sumo account preferences, do the following:

1. At the very bottom of the Left Nav Bar, click your Account Name.
1. In the pop-up dialog, select **Preferences**.

    ![WTS_Preferences_LeftNav-option.png](/img/get-started/ui/WTS_Preferences_LeftNav-option.png)

1. In the Preferences page that appears on the right, you can modify settings in the following areas:

    * **My Profile**: username and password
    * **My Security Settings**: enable and disable 2-step verification
    * **My Access Keys**: add, edit, and remove access keys
    * **My Preferences**: your account session settings

For more information, see the [Preferences Page](manage-account.md).

### Get help: docs, community, and more

Whenever you have a question, there are a number of ways in which you can get the answers you need:

* Check out the **[Release Notes](/release-notes)**
* Search documentation
* Visit the **Learn Page** in the Sumo Logic UI
* Post a question on the [**Sumo Logic Community**](https://support.sumologic.com/hc/en-us/community/topics)
* Contact [**Support**](https://support.sumologic.com/)
* Try our **Customer Slack** channel

:::sumo Getting Help
See [Getting Help and Contacts](help-menu.md) for full information.
:::

### Admin: Manage data collection, data settings, and alerts

Sumo Logic Administrators (Admins) are responsible for managing data collection, data settings, and alerts for their organization. You must have Sumo Logic Admin role privileges to perform these tasks.

To manage data in Sumo Logic, do the following:

1. Go to the **Left Nav Bar** and click **Manage Data**.

    ![manage-data.png](/img/get-started/ui/manage-data.png)

1. Choose from the following, as needed:

    * **Collection.** [Manage collectors and sources](/docs/manage/collection).
    * **Logs.** Manage [fields] (../Manage/Fields.md "Fields"), [field extraction rules] (../Manage/Field-Extractions.md "https://help.sumologic.com/Manage/Search_Optimization_Tools/Manage_Field_Extractions"), [partitions] (../Manage/Partitions_and_Data_Tiers.md "https://help.sumologic.com/Manage/Search_Optimization_Tools/Manage_Partitions"), [scheduled views] (../Manage/Scheduled-Views.md "Manage Scheduled Views"), [connections](/docs/manage/connections-and-integrations), and [data forwarding] (../Manage/Data-Forwarding.md "Data Forwarding").
    * **Metrics.** Manage metrics rules, [logs-to-metrics] (../Metrics/Logs-to-Metrics.md "Logs-to-Metrics"), and [metrics transformation rules] (../Metrics/Metrics_Transformation_Rules.md "Metrics Transformation Rules").
    * **Alerts.** [Monitors](/docs/monitors), [connections](/docs/manage/connections-and-integrations), and [health events] (../Manage/Health_Events.md "Health Events").

### Admin: Manage accounts, users, and security

Sumo Logic administrators (admins) manage user accounts, user roles, and security. You must have Sumo Logic Admin role privileges to perform these tasks.

To administer Sumo Logic accounts, users, and security, do the following:

1. Go to the **Left Nav Bar** and click **Administration**.

![WTS_UI_Administration_menu-options.png](/img/get-started/ui/WTS_UI_Administration_menu-options.png)

1. Choose from the following, as needed:

    * **Account.** [View information about your organization's Sumo Logic subscription] (../Manage/01Manage_Subscription.md "https://help.sumologic.com/Manage/01Account_Usage"), [enable and manage the data volume index,] (../Manage/Ingestion-and-Volume/Data_Volume_Index.md "https://help.sumologic.com/Manage/Ingestion_and_Volume/Enable_and_Manage_the_Data_Volume_Index") [manage billing] (../Manage/01Manage_Subscription.md "https://help.sumologic.com/Manage/01Account_Usage").
    * **Users and Roles**. [Manage users and roles] (../Manage/Users-and-Roles.md "https://help.sumologic.com/Manage/Users_and_Roles").
    * **Security.** [Set password policy for your org] (../Manage/Security/Set-the-Password-Policy.md "Set the Password Policy"), [set up security whitelist] (../Manage/Security/Create-an-Allowlist-for-IP-or-CIDR-Addresses.md "Create a Whitelist for IP or CIDR Addresses"), [manage access keys] (../Manage/Security/Access-Keys.md "https://help.sumologic.com/Manage/Security/Access_Keys"), manage security polices ([audit index] (../Manage/Security/Audit-Index.md "https://help.sumologic.com/Manage/Security/Enable_and_Manage_the_Audit_Index"), [support account access,] (../Manage/Security/Enable-a-Support-Account.md "Enable a Support Account") and [dashboard sharing](../dashboards-new/share-dashboard-new.md), and [set up SAML authentication] (../Manage/Security/SAML.md "https://help.sumologic.com/Manage/Security/SAML").

## Become a Sumo Pro user

Now that you're familiar with the layout and features in the Sumo Logic user interface (UI), you're ready to ramp up your Sumo skills with [self-paced training](https://www.sumologic.com/self-paced-training/).

You don't have to stop there either. You can take the next step and become Sumo Certified. For more information on the Sumo Logic Certification program courses, go to the **Home** page and click the **Certification** tab. See [Certification FAQs](certification-faqs.md) for more information.

![WTS_UI_Certification.png](/img/get-started/ui/WTS_UI_Certification.png)
