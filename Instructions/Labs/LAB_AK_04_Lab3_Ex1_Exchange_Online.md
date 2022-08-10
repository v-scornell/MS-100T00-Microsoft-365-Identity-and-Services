# Module 4 - Lab 3 - Exercise 1 - Review Key Features of Exchange Online

Holly Dickson is Adatum’s Enterprise Administrator. She has recently deployed
Microsoft 365 in a virtualized lab environment. Now that she has a tenant
account set up and has been assigned to the Global Administrator role, she has
been asked to review the key administrative functions within Exchange Online,
SharePoint Online, and Teams. This task will enable her to become familiar with their
functionality and can offer guidance to her IT team on how these services can be used
throughout Adatum.

Regarding Microsoft Exchange, Adatum’s CTO has requested that Holly review some
of the basic administrative functions in Exchange Online related to mail flow
and recipient management. Since the Global Administrator role includes the
Exchange Administrator role, Holly can perform all Exchange-related tasks.

### Task 1 – Manage Recipients

As you continue in your role as Holly Dickson, you are ready to review the steps
involved in creating and managing mail flow recipients.

1.  At the end of the previous lab, you were on LON-CL1, where you took on the
    role of Laura Atkins and installed Microsoft 365 Apps for enterprise. For
    this lab exercise, you must switch back to LON-DC1, where you will resume
    your pilot project in the role of Holly Dickson. <br/>

    Switch to **LON-DC1**, where you should still be logged in as the
    **Administrator** with a password of **Pa55w.rd**; if not, then do so now.

2.  You should still have an Edge browser session and the Microsoft 365 admin
    center open from the prior lab. If so, proceed to the next step; otherwise,
    open Microsoft Edge, navigate to **https://portal.office.com/**, log in as
    **Holly@xxxxxZZZZZZ.onmicrosoft.com** (where xxxxxZZZZZZ is the tenant prefix provided by your lab hosting
    provider) and **Pa55w.rd**, select the **App launcher** icon (the square made up of 3 rows of dots) that appears above the **Home** icon in the top left corner of the screen, and then in the **Apps** pane that appears, select **Admin**; this opens the **Microsoft 365 admin center** in a new browser tab.

3.  In the **Microsoft 365 admin center**, select **Show all** (if necessary) in the navigation pane, then scroll down to **Admin centers**
    and select **Exchange**. This will open the **Exchange admin center** in a
    new tab. This is the Exchange admin center for Microsoft Exchange Online. <br/>

	**Note:** If a **Learn about the new menu** window appears, select the **X** to close it.

4.  In the **Exchange admin center**, select **Recipients** in the navigation pane to expand the Recipients group.

5.  In the **Recipients** group, select **Mailboxes**. The mailboxes that appear
    in this view include all the user accounts that were created in your
    tenant by the lab hosting provider, along with the mailboxes for Holly
    Dickson and Laura Atkins that were created when you added their Microsoft
    365 user accounts in previous labs. <br/>

    Select the mailbox for **Joni Sherman** by selecting her **Display name**
    This will open Joni's **User mailbox** window. By
    default, the window displays the **Mailbox** tab (the tabs appear at the top
    under Joni’s name).

6.  Towards the bottom of the **Mailbox** tab, under the **More actions** section, select
    **Custom attributes**.

7.  This opens the **Custom attributes** window for Joni. You can enter up to 15
    attributes. You will not be entering any attributes in this lab exercise,
    but it’s important that you know this feature is available. Select the **back arrow** in the top left corner of the pane to return to the previous page, which is Joni Sherman's properties page.  <br/>

    ‎**Note:** Custom attributes are properties your company can use for specific
    mailbox identification, such as a cost center number for the mailbox or
    other information such as an HR personnel number.

8.  This returns you to the **Mailbox** tab in Joni's User mailbox pane. Select the **Account** tab, which
    enables you to maintain additional information for this mailbox. While you
    won’t enter any of this optional information for this lab, take a few
    minutes now and select the following links to see what additional
    information can be captured.  <br/>

    -   **Manage contact information.** This window enables you to add
        additional contact information, such as the user’s personal address and
        Home and Mobile phone numbers.

    -   **Manage Organization information.** This window enables you to add
        company-specific information such as Title, Department, and Company.

9.  Select the **Mailbox** tab again, and then under the **Mailbox permissions**
    group, select **Manage mailbox delegation.**  <br/>

	The **Manage mailbox delegation for Joni Sherman** window enables the admin to
    assign a user to this mailbox’s **Send as** and **Send on behalf**
    permissions, as well as **Read and manage (Full Access**.  

10. For this lab, you will assign **Read and manage (Full Access)** permission to Holly Dickson. This will enable Holly to open Joni's mailbox and perform all mailbox functions, just as if she were Joni. <br/>

	In the **Manage mailbox delegation for Joni Sherman** window, select the **Edit** button that appears below the **Read and manage (Full Access)** section.

11. In the **Manage Mailbox delegation** window, select **+Add members**.

12. In the **Add read and manage permissions** pane, select **Holly Dickson**
    from the list of user accounts, and then select the **Save** button. Then
    select **Confirm.** 

13. Once you receive the message indicating **Mailbox permissions were added to these mailboxes**, select the **X** in the upper right corner of this pane to close it. <br/> 

    ‎**Note:** After about an hour Holly Dickson will have access Joni’s mailbox
    without needing a password.

14. Leave your browser and all the tabs open for the next task.

### Task 2 – Manage Groups

In this task you will create two types of groups within Exchange Online. The
first is a distribution list of email recipients, which is used to create a
one-stop email list for contacting users simultaneously rather than having to
email each recipient individually. The second type of group is a Microsoft 365
group.

1.  Your browser should still be open to the **Exchange admin center** from the
    prior task. In the navigation pane, under the **Recipients** group, select **Groups**.  <br/>

	**Note:** The **Groups** page displays a tab for each type of group that can be
    maintained. The **Microsoft 365** tab is displayed by default, which
    displays all the Microsoft 365 groups. This list should include the **Inside Sales** group that you created in
        Lab 2. In the following steps, you will create a distribution list group and a Microsoft
    365 group whose email addresses will be in Microsoft 365 (@xxxxxZZZZZZ.onmicrosoft.com).

2.  On the **Groups** page, select **Add a group**, which
    initiates the **Add a group** wizard.

3.  In the **Add a group** wizard, the steps to add a group are displayed in the
    middle pane. In the **Choose a group type** pane on the right, select
    **Distribution** and then select **Next**.

4.  In the **Set up the basics** page, enter **Sales Department** in the
    **Name** field, tab into the **Description** field (which enables the
    **Next** button) but leave the field blank, and then select **Next**.

5.  In the **Edit settings** page, enter the following information and then
    select **Next.**  <br/>

    -   Group email address: **SalesDept**

    -   In the domain field to the right of the Group email address, select the
        drop-down arrow and select **xxxxxZZZZZZ.onmicrosoft.com** (where
        xxxxxZZZZZZ is the tenant prefix provided by your lab hosting provider).

    -   Joining the group: Select **Owner approval.** This option allows the
        owner to control who can join the group.

    -   Leaving the group: Select **Closed.** This option allows the owner to
        control who can leave the group. Together with joining the group, you
        can control who joins or leaves your distribution group.   
        
        **Note:** In a real-world scenario, if you want less administration
        governing group membership, then select **Open** for either of these two
        options.

6.  On the **Review and finish adding group** page, review the information that
    you entered for this group. If anything needs to be changed, select the
    appropriate **Edit** link and make your corrections. When everything is
    correct, select the **Create group** button.

7.  Once the group is created, the **Sales Department is created** page appears.
    Note the message at the top of the page indicating that it can take up to an
    hour for the group to appear in your groups list. Select **Close**.

8.  This should return you to the **Groups** page, which is currently displaying
    the **Microsoft 365** tab. Select the **Distribution list** tab to see the
    distribution group that you just created. If **Sales Department** does not
    appear in the list of distribution groups, refresh the page every few minutes
    until the group appears.

9.  Once the **Sales Department** group appears in the list, select the **Sales
    Department** name. This opens a detail pane for the Sales Department group.
    The **General** tab is displayed by default. You now want to add
    members to this group, so select the **Members** tab.

10. On the **Members** tab, under the **Owners** section, select **View all and manage owners**, which opens
    the **Owners** window. Since you are logged into the Exchange admin center
    using Holly Dickson, her account was assigned as the default Owner when you created the group. However,
    Holly wants Alex Wilber to co-own the group along with her, so select **+Add owners**.

11. In the **Add owners** window, select **Alex Wilber**, and then select the
    **Add (1)** button. This returns you to the **Owners** window and displays
    Alex and Holly as owners of this group. Select the back arrow in the
    top-left corner of the window to return you to the **Sales Department**
    window.

12. Under the **Members** section, select **View all and manage members**, which opens the **Members** window.
    Select **+Add members**.

13. In the **Add members** window, select **Allan DeYoung**, **Diego
    Siciliani,** and **Lynne Robbins**, and then select the **Add (3)** button. <br/>

	This returns you to the **Members** window and displays Lynne, Allan, and
    Diego as members of this group. Select the back arrow in the top-left corner
    of the window to return you to the **Sales Department** window.

14. In the **Sales Department** window, the owners and members that you added
    should be displayed. Select the **Settings** tab. While this tab enables you to
    make advanced settings changes, you won't make any settings changes in this lab.  <br/>

	However, review the settings that can be updated here for future reference. Once you
    have reviewed the settings, select the **X** in the top right-hand corner of
    the window to close it.

15. This should return you to the **Groups** page, which is currently displaying
    the **Distribution list** tab. You will now add a dynamic distribution group, so select **Add a group**. This initiates the **Add a group** wizard.

16. In the **Add a group** wizard, the steps to add a group are displayed in the
    middle pane. In the **Choose a group type** pane, select
    **Dynamic distribution** and then select **Next**.

17. On the **Set up the basics** page, enter the following information and
    then select **Next**: <br/>

    -   Name: **Dynamics CRM project team**

    -   Description: **Adatum users working on the Microsoft Dynamics CRM project**

18. On the **Assign users** page, enter the following information and then
    select **Next**: <br/>

    -   Owner: select **Holly Dickson**

    -   Members: select **Only the following recipient types**

    -   Select the **Users with Exchange Mailboxes** check box.

    -   Membership in this group will be determined by the rules you set below:

        -   Select condition: **Department**

        -   Enter words, separate with commas: type the word **Sales**

19. On the **Edit settings** page, enter the following information then select
    **Next:** <br/>

    -   Group email address: **DynCRM**

    -   Group email address domain: In the domain field to the right of the
        **DynCRM** alias, select the drop-down arrow and select
        **xxxxxZZZZZZ.onmicrosoft.com** (where xxxxxZZZZZZ is the tenant prefix
        provided by your lab hosting provider.

20. On the **Review and finish adding group** page, review the information that
    you entered for this group. If anything needs to be changed, select the
    appropriate **Edit** link and make your corrections. When everything is
    correct, select the **Create group** button.

21. Once the group is created, the **Dynamics CRM Project Team is created, but it isn't ready to use yet** page
    appears. Note the message that it may take up to 2 hours until you can send a message to this group. Select **Close**.

21. This should return you to the **Groups** page. Select the **Dynamic Distribution list** tab. If **Dynamics
    CRM Project Team** does not appear in the list of dynamic distribution
    groups, refresh the list (select the **Refresh** option on the menu bar) every few minutes until the group appears.

23. Holly now wants to add Nestor Wilke as an owner of this Dynamics CRM project team group. Perform the
    same steps that you completed earlier when you added an owner to the Sales
    Department group. In this case, add **Nestor Wilke** as a co-owner of the
    **Dynamics CRM Project Team** group.

24. This should return you to the **Groups** page, which is currently displaying
    the **Dynamic Distribution list** tab. Select the **Dynamics
    CRM Project Team**, and in the detail pane that opens for the group, select the **Members** tab. <br/>

	**Important:** Instead of having two owners (Holly and Nestor), verify that only Nestor appears as the owner of the group. A dynamic distribution group is different from the other group types because it can only have one owner. So when you added Nestor as a group owner in the earlier step, what actually happened is that Nestor replaced Holly as sole owner of the group. 
	
26. Close the **Dynamics CRM project team** pane.

27. Leave your browser and all tabs open for the next task.

### Task 3 - Upgrade Distribution Lists

Organizations have typically relied on distribution groups in Exchange to
communicate and collaborate with groups of people both inside and outside the
company. However, Microsoft 365 groups offer a more powerful solution for
collaboration, and Adatum’s CTO wants to take advantage of this feature. He has
asked Holly to upgrade the company’s Sales Department distribution list to a
Microsoft 365 group so that Adatum’s Sales staff can choose the people they want
to collaborate with and easily set up a collection of resources for those people
to share.

1.  Your browser should still be open to the **Exchange admin center** from the
    prior task, and it should still be displaying the **Groups** window and the
    **Dynamic distribution list** tab. In the **Groups** window, select the
    **Distribution list** tab.

2.  Select the check box to the left of the **Sales Department** distribution list
    and then select **Upgrade distribution group** in the menu bar.

3.  A **Ready to upgrade** pop up window will appear. Select the **Upgrade**
    button to upgrade the group from a distribution list to a Microsoft 365
    group.

4.  Select the **Microsoft 365** tab. This may take up to 5 minutes for the
    upgrade to complete, at which time the Sales Department group will appear in
    the list of Microsoft 365 groups. You may need to select **Refresh** on the
    menu bar every few minutes before the Sales Department group appears. <br/>

	If necessary, continue with the next task while you wait for the Sales Department to appear in the list of Microsoft 365 groups.

### Task 4 - Configure a Group Naming Policy

A group naming policy enables organizations to standardize and manage the names
of distribution groups created by its users. You can require that a specific
prefix and suffix be added to the name for a distribution group at the time it’s
created, and you can also block specific words from being used. This helps
organizations minimize the use of inappropriate words in group names.

Adatum’s CTO wants Holly to implement a standard group naming policy throughout the
organization based on the following format: **{Department} Group: {Group Name} {City}**

1.  Your browser should still be open to the **Exchange admin center** from the
    prior task, and it should still be displaying the **Groups** window and the
    **Microsoft 365** tab. In the menu bar that appears over the list of groups,
    select **Add naming policy.**

2.  In the **Edit group naming policy** window that appears, the **Policy** tab
    is displayed by default. Under the **Create a policy** section, you can
    select a prefix and a suffix. <br/>

    In the **Choose a prefix to add to the beginning of the group names**
    section, you will define the prefix values that will be displayed BEFORE the group name. Remember, the group naming policy will be: **{Department} Group: {Group Name} {City}** <br/>

	So the prefix that you will define in this section will be the values displayed BEFORE **{Group Name}**. This will be the Department and the text string "Group:". <br/>

	The Department is a tenant attribute. The first prefix field is prefilled with **Attribute**, so do NOT change this field. However, you need to select the Department attribute, so select the **Select one** field and then select
    **Department** from the drop-down list.

3.  The second portion of the prefix that will appear before the **{Group Name}** is the text "Group:". To define this portion of the prefix, select **Add prefix**, which appears below the **Attribute** field. This option displays another set of prefix fields. 

4.  In this second set of prefix fields, the first field is again set to **Attribute** by default.
    However, this second portion or the prefix won't be an attribute, but rather a text string. So select this **Attribute** field and then select **Text** from the drop-down list that appears. <br/>

	Then in the **Add text** field that appears to the right of the **Text** field, enter **Group:**.

5.  You're now ready to define the suffix portion of your group naming policy. The suffix is what appears AFTER the **{Group Name}**. For your group naming policy, this will be the City attribute. <br/>

	The first suffix field is prefilled with **Attribute**, so do NOT change this field. However, you need to select the City attribute, so select the **Select one** field and then select
    **City** from the drop-down list.

6.  At the bottom of the **Edit group naming policy** pane, review the **Preview policy** example that is
    based on the parameters you selected. The format should appear as: <br/>
    
    	**<Department>Group:<GroupName><City>**  <br/>

	If any portion of this rule in incorrect and must be fixed, select the
    correct values now. When everything is correct, select the **Save**
    button at the bottom of the pane.

7.  Once the group naming policy changes have been saved, close the **Edit group
    naming policy** pane. Leave all your browser tabs open for the next task.

### Task 5 – Manage Resources

A room mailbox is a resource mailbox that is assigned to a physical location,
such as a conference room, an auditorium, or a training room. Users can easily
reserve these rooms by including room mailboxes in their meeting requests.
Adatum’s CTO wants to test this feature using the company’s most popular
conference room, and he has asked Holly to configure this resource.

**Note:** Creating a resource record for a room in your office is designed for
administrators to set up a meeting location for booking. When scheduling
meetings, you can select the room from the Global Address List (GAL).

1.  Your browser should still be open to the **Exchange admin center** from the
    prior task, and it should still be displaying the **Groups** window. In the
   navigation pane, under the **Recipients** group, select **Resources.**

2.  In the **Resources** window, select **+Add a resource** on the menu bar.
    This initiates the **New resource mailbox** wizard.

3.  In the **New resource mailbox** wizard, on the **Fill in the basic info**
    page, select **Room**, and then enter the following information:  <br/>

    -   Name: **Conference Room 1**

    -   Resource email: **Con1**

    -   Email address domain: In the domain field to the right of the **Con1**
        alias, select the drop-down arrow and select
        **xxxxxZZZZZZ.onmicrosoft.com** (where xxxxxZZZZZZ is the tenant prefix
        provided by your lab hosting provider

    -   Capacity: **15**

    -   Location: The room is in Building 5, Room 2011, so enter **5/2011**

    -   Phone: **425-555-2011**

4.  Select **Next.**

5.  A second **Fill in the basic info** page appears. This page is used to enter
    the resource address. Since this information isn't applicable to the conference room, you can skip this page and select **Next**.

6.  In the **Booking options** page, select the **Allow scheduling only during
    working hours** check box.

7.  Uncheck (clear) the **Auto-accepts meeting request** check box.

8.  In the **Booking delegates** field, enter **Holly** and then select **Holly
    Dickson**. Then enter **Nestor** and select **Nestor Wilke**. <br/>

    **Note:** This option allows a user to filter booking requests.

9.  Ensure the check box next to **Automatically decline meetings outside of
    limits below** is selected or you won’t be able to input the following
    information.

10. In the **Booking window (days)** field, enter **60**. <br/>

    ‎**Note:** As a best practice, organizations should establish a company
    standard so that events do not over-book locations.

11. In the **Maximum duration (hours)** field, enter **120** (this is five days,
    or one work week).

12. Select **Next**.

13. On the **Review resource** page, review the resource information that you
    just entered. If anything needs to be fixed, select the **Back** button and
    make the necessary corrections. When everything looks correct, select
    **Create** and wait for the resource to be created. A message is displayed on the **Status** page indicating it may take a couple of
    minutes to create the resource.

14. Once the resource mailbox has been successfully created, select **Done**. The new resource record for **Conference Room
    1** should appear in the **Resources** window.

15. Leave your browser and all tabs open for the next task.

### Task 6 – Manage Contacts

One of the key features of Exchange Online is the ability to maintain different
types of contacts in the Exchange Admin Center. In this task, you will be
introduced to mail contacts and mail users.

1.  Your browser should still be open to the **Exchange admin center** from the
    prior task, and it should still be displaying the **Resources** window. In
    the navigation pane, under the **Recipients** group, select
    **Contacts.**

2.  In the **Contacts** window, select **+Add a contact** that appears on the
    menu bar.

3.  In the **Add contact** pane that appears on the right, enter the following
    information: <br/>

    -   Contact type: select **Mail contact** from the drop-down menu  <br/>

        ‎**Note:** This option enables external people from outside your
        organization to be added to your Exchange Online distribution lists. This is what you will do in this step - add Hai Chu from Fabrikam as a mail contact.<br/>

    -   First name: **Hai**

    -   Last Name: **Chu**

    -   Display Name: tab into the field and **Hai Chu** is automatically
        displayed

    -   External Email Address: **Hai@fabrikam.com**

    -   Company: **Fabrikam**

4.  Select the **Add** button at the bottom of the pane. It may take a minute or two to successfully create the
    record.

5.  Once the Contact record has been successfully created, a message indicating the **Contact created
    successfully** will appear. Select the **X** in the upper right corner to close the pane. Hai Chu should now appear
    in the **Contacts** window. If Hai Chu doesn’t appear, select **Refresh** on
    the menu bar to refresh the Contacts list until the record appears (it may take a few minutes).

6.  Hai Chu’s contact record was for a Mail Contact. Holly now wants to create a
    second contact, but this time for a Mail User. On the menu bar above the
    Contacts list, select **+Add a contact** to add another contact. <br/>
    
    	**Note:** A Mail User is an individual who needs to use the company
        domain even though they are not a full-time employee (for example, contractors, advisors, and selective temporary staff). Defining a Mail User will
        forward email to the individual’s external email when mail is sent to
        the contact’s internal company account.  <br/>

        ‎**WARNING**: A Mail User does not need a license to access SharePoint
        Online; the user simply needs to be given access to it.  <br/>

7.  In the **Add contact** pane that appears on the right, enter the following
    information: <br/>

    -   Contact type: **Mail user** (this should be selected by default) <br/>

    -   First name: **Bill**

    -   Last Name: **Norman**

    -   Display Name: tab into the field and **Bill Norman** is automatically
        displayed.

    -   External email address:
        **Bill@fabrikam.com**

    -   Alias: **Bill**

    -   User ID: **Bill** (this is the user’s alias for his internal Adatum
        account.

    -   Domain: in the domain field to the right of the User ID, select the
        drop-down arrow and select **xxxxxZZZZZZ.onmicrosoft.com** (where
        xxxxxZZZZZZ is the tenant prefix provided by your lab hosting provider.

    -   Password: **Pa55w.rd**

    -   Confirm: **Pa55w.rd**

8.  Select **Add.**

9.  Once the Contact record has been successfully created, a message indicating the **Contact created
    successfully** will appear. Select the **X** in the upper right corner to close the pane. Select **Close**. 

10. Bill Norman should now
    appear in the **Contacts** window. If Bill Norman doesn’t appear, select
    **Refresh** on the menu bar to refresh the Contacts list until his record
    appears. 

11. Leave the Exchange admin center tab open and proceed to the next task.

### Task 7 – Configure Messaging Protection

Adatum has experienced a recent rash of malware infections. The company’s CTO
has asked Holly Dickson to investigate the various options that are available in
Exchange Online to protect Adatum’s messaging environment. In these next three tasks, you will configure malware, connection, and
spam policies, respectively. 

**Warning:** To create these policies, you must be assigned the **Organization
Management** role, which the MOD Administrator will assign to Holly at the start of this task. You will log in to Microsoft 365 as the MOD Administrator and assign Holly this permission. However, it sometimes takes an hour or so for the role permissions to propagate
through the system. This is due to the replication process that occurs within
the system. In the Microsoft data centers, certain objects are consolidated to
save space. You may encounter this delay when you assign RBAC roles in Microsoft 365 Defender, or when you use Exchange Online PowerShell or
the Exchange admin center to change one of these objects for the first time.

Therefore, when you sign into Microsoft 365 as Holly later in this task and create the malware policy, you may receive a **Client Error** that indicates an error
occurred when creating the policy. This error occurs because the Organization
Management permissions haven’t fully propagated through the system for Holly. To
work around this, you will be provided with PowerShell instructions that will
enable you to customize organization management objects.

You will perform this task in LON-CL1. 

1.  Switch to **LON-CL1** in your VM environment.   

2.  You should still be logged into LON-CL1 as the **Administrator** with a
    password of **Pa55w.rd** from the prior lab that used LON-CL1. If a Microsoft Teams window appers, close it now. <br/>

	 You must sign into Microsoft 365 as the MOD Administrator, who will later assign Holly the Organization Management role.To sign in to Microsoft 365 as the MOD Administrator, begin by selecting the **Edge** browser icon on the taskbar. In your **Edge** browser, navigate to the **Office 365 home** page by entering **https://portal.office.com**, sign-in as the MOD Administrator account (**admin@xxxxxZZZZZZ.onmicrosoft.com**, where xxxxxZZZZZZ is the tenant prefix provided by your lab hosting provider), and enter the tenant admin password provided by the lab hosting provider. <br/>

	In the **Office 365 Home** page, navigate to the **Microsoft 365 admin center**.

3. In the **Microsoft 365 admin center**, select **Show all** in the navigation pane, and then under **Admin centers**, select **Security**. This opens the **Microsoft 365 Defender** portal in a new tab.

4.  In the **Microsoft 365 Defender** portal, scroll down towards the bottom of the 
    navigation pane and select **Permissions & roles**.

5.  In the **Permissions** page, there are two groups - Azure AD, and Email & collaboration roles. Under the **Email & collaboration roles** group, select **Roles**. 

6. In the **Permissions > Permissions** page, locate the **Search** field on the menu bar (it appears to the right of the **Refresh** option). Enter **org** in the **Search** field
    and then select the magnifying glass icon. This is a quick way to display
    the Organization Management role group so that you don’t have to scroll
    through a list of roles to find it. <br/>
    
    The search will display the **Organization Management** role, which is the
    only role starting with **org**. Select the **Organization Management** role to
    display the details for this role group.

7.  In the **Organization Management** pane that appears on the right, scroll
    down to the **Members** section at the bottom of the pane. To the right of the
    **Members** section, select **Edit**.

8.  On the **Editing Choose members** page, select **Choose members**.

9.  On the **Choose members** page, select the **+Add** button.

10. On the **Choose members** page, you will choose which users will be added as members of this role. In the list of users that appears under **Members**, select the check box next to **Holly Dickson** and then select **Add**.

11. On the **Choose members** page, Holly should appear in the list of members
    for this role. Select **Done**.

12. On the **Editing Choose members** page, select **Save**.

13. On the **Organization Management** pane, select **Close**.

14. On **LON-CL1**, you must log out of Microsoft 365 as the MOD Administrator and log back in as Holly Dickson. On the **Microsoft 365 Defender** portal, select the **MA** circle in the upper-right corner of the screen, and in the **MOD Administrator** window that appears, select **Sign out**.

15.  Once you're signed out, close your Edge browser. This will ensure that when you reopen Edge and sign into Microsoft 365, the Microsoft 365 admin center will use the newly signed in credentials for Holly rather than opening it for the MOD Administrator, which was stored in the browser's cache.

16.  Select the **Edge** icon on your taskbar to re-open the Edge browser. Enter **https://portal.office.com** in the address bar to open the Office 365 home page.

17.  In the **Pick an account** window that appears, select Holly's email address (**Holly@xxxxxZZZZZZ.onmicrosoft.com**, where xxxxxZZZZZZ is the tenant prefix provided by your lab hosting provider). In the **Enter password** window, enter **Pa55w.rd** and then select **Sign in**. If the **Stay signed in?** window appears, select the **Don't show this again** check box and then select **Yes**.

17.  On the **Microsoft Office Home** page, navigate to the **Microsoft 365 admin center**. 

18.  In the **Microsoft 365 admin center**, select **Show all** in the navigation pane, and then under the **Admin centers** section, select **Security**. This opens the Microsoft 365 Defender portal in a new tab.

19. In the **Microsoft 365 Defender** navigation pane, under the **Email & collaboration** section, select **Policies & rules**.

20. In the **Policies & rules** page, select **Threat policies**.

21. In the **Threat policies** page, under the **Policies** section, select **Anti-malware**.

22. In the **Policies & rules > Threat policies > Anti-malware** page, on the menu bar at the top
    of the window, select **+Create** to add a new malware filter. This starts
    the **Create a new anti-malware policy** wizard.

23. In the **Name your policy** page, enter **Malware Policy** in the **Name**
    field.

24. In the **Description** field, enter **This policy has been created to protect Adatum’s messaging environment** and then select **Next**.

25. In the **Users and domains** page, enter **onmicrosoft** in the
    **Domains** field. This will display the list of Adatum domains containing
    **onmicrosoft.com**. Select the **M365xZZZZZZ.onmicrosoft.com** domain
    that’s displayed and then select **Next**.

26. On the **Protection settings** page, under the **Protection settings**
    group, select the check boxes for the following settings: <br/>

    -   **Enable the common attachments filter** (if it’s not already selected)

    -   **Enable zero-hour auto purge for malware (recommended)**.

27. In the **Notification** section, do not select any of the notification
    options since you don't want to generate any notifications with this policy. Select **Next**.

28. On the **Review** page, review all the information for this malware policy.
    If anything needs to be changed, select the **Back** button and make the
    necessary corrections. When all the information is correct, select
    **Submit**.

29. If the anti-malware policy was successfully created, then skip to the next
    step.   <br/>
    
    However, if you receive a **Client Error** dialog box that indicates an
    error occurred when creating the policy, then the permissions assigned to
    Holly through the Organization Management role haven’t fully propagated
    through the system. For this lab, instead of waiting an hour or so for this
    permission replication to occur, select **OK** in this dialog box and then
    perform the following PowerShell commands that will enable you to customize organization
    management objects. Once you’ve completed these steps, you will resubmit the
    **Review** page to save the malware policy that you just created. <br/>

    1.  On LON-CL1, you must open an elevated instance of **Windows
        PowerShell**. Select the magnifying glass (Search) icon on the taskbar
        at the bottom of the screen ad type **powershell** in the Search box
        that appears. In the list of search results, right-click on **Windows
        PowerShell** (do NOT select Windows PowerShell ISE) and select **Run as
        administrator** in the drop-down menu.

    2.  Maximize your PowerShell window. In Windows PowerShell, at the command
        prompt, type the following command and press Enter:

        	Install-Module -name Exchangeonlinemanagement

    3. If you are prompted to confirm whether you want to install the module from
    an untrusted repository (PSGallery), enter **A** to select **[A] Yes to
    All.**

    4. At the command prompt, type the following command and press Enter:

   		Connect-exchangeonline

    5.  A **Microsoft 365 Sign in** window will appear. Enter the username for
    the **Mod Administrator** account, which is the Microsoft 365 tenant admin account provided by your learning provider
    (admin@M365xZZZZZZ.onmicrosoft.com) and then select **Next**.

    6.  In the **Enter password** window, enter the password provided by your learning provider for this tenant admin account, and then select **Sign in**. It may take
    a moment to sign in before it returns a command prompt.

    7.  At the command prompt, type the following command and press Enter (**Note:**
    This command may fail the first time. If it fails, re-run this step until it
    returns a successful result (the command prompt appears with no errors);
    testing shows that it sometimes takes two attempts):

		Enable-OrganizationCustomization

    8.  Close the PowerShell window.

    9.  Return to your **Edge** browser and the **Review** page for your new
    anti-malware policy. Select **Submit** to resubmit your anti-malware policy.
    This time the policy should be successfully saved.

30. On the **Created new anti-malware policy** page, it indicates the new policy
    has been created and will go into effect immediately. Select **Done.** 

   	**Note**: If a dialog box appears with a message that
	indicates your organization settings need to be updated, select **Yes** to
	continue. It may take a minute for your organization settings to be updated.

31. Leave your browser open for the next task.


### Task 8 – Manage Connection Filters

Holly has been contacted by Adatum’s CTO, who's upset that he keeps finding
email from friends and business associates in his junk email folder. He’s
even had email blocked entirely by a spam filter. He has asked Holly to address
this problem by making sure that email sent from people who are trusted doesn’t
become blocked.

Holly has investigated the situation and has found that in Microsoft 365, you
can create a connection filter policy that defines a list of IP addresses that you
trust. This is known as an Allow list, or Safe Sender list. You can also create
a Blocked senders list, which is a list of IP addresses (typically from known
spammers) that you never want to receive email messages from.

1.  You should still be logged into Microsoft 365 as Holly Dickson after completing the prior task. Your Edge browser should still be in the **Microsoft 365 Defender** portal on the **Policies & rules > Threat policies > Anti-malware** window. 

2.  In the **Policies & rules > Threat policies > Anti-malware** navigation thread at the top of the page, select **Threat policies**.

3.  In the **Threat policies** window, under the **Policies** section, select
    **Anti-spam**.

4.  The **Policies & rules > Threat policies > Anti-spam policies** window displays a list of
    default **Anti-spam policies** that control how messages are handled by
    Microsoft 365 anti-spam policies. <br/>

    In the list of policies, select the **Connection filter policy (Default)**.
    This displays the current settings for this default spam filter in the
    right-hand pane.

5.  In the **Connection filter policy (Default)** pane, the **Connection
    filtering** section displays options regarding which IP Addresses may send
    messages to your environment and which IP addresses will be blocked from
    sending messages. <br/>

    **Important:** You will **NOT** be adding IP addresses to the allow or block lists. You can do
    this if you have a known IP address you would like to test against. It
    typically takes up to 1 hour to propagate the change within the system. For
    this lab, simply review the fact that you can create allowed and blocked
    lists of IP addresses.

6.  At the bottom of the **Connection filtering** section, select the **Edit
    connection filter policy** link.

7.  In the **Connection filter policy (Default)** pane, select the **Turn on
    safe list** check box. This is a best practice that enables for your tenant the most common third-party sources of trusted senders that Microsoft
    subscribes to. Selecting this check box skips spam filtering on messages
    sent from these senders, ensuring they are never mistakenly marked as spam.

8.  Select **Save** to save this filter, and then select **Close** once the
    changes are successfully saved.

9. Leave your Edge browser open to the **Microsoft 365 Defender** portal for the next task.

### Task 9 – Manage Spam Filters

For Microsoft 365 customers whose mailboxes are hosted in Microsoft Exchange
Online, their email messages are automatically protected against spam and
malware. Microsoft 365 has built-in malware and spam filtering capabilities that
help protect inbound and outbound messages from malicious software and help
protect you from spam.

As Adatum’s Global Administrator, Holly doesn’t need to set up or maintain the filtering
technologies, which are enabled by default. However, she can make
company-specific filtering customizations in the Microsoft 365 Defender portal.
Holly has decided to test this out by configuring a spam policy to grant or deny
an email by focusing on the language of the email and the location of the
email’s origin.

1.  In the **Microsoft 365 Defender** portal, the **Policies & rules > Threat policies > Anti-spam policies** window should still be displayed after having completed
    the prior task. <br/>

    In the list of anti-spam policies, select the **Anti-spam inbound policy (Default)**.

2.  In the **Anti-spam inbound policy (Default)** pane that appears, take a
    moment and review the policy settings that are available in this filter.
    There are three sections of settings – **Bulk email threshold & spam
    properties**, **Actions**, and **Allowed and blocked senders and domains**.

3.  Once you’ve finished reviewing these settings, scroll to the bottom of the
    **Bulk email threshold & spam properties** section and select the **Edit
    spam threshold and properties** link.

4.  In the **Spam threshold and properties** pane that appears, scroll to the top of the pane. The **Bulk email
    threshold** at the top of the pane is set to **7** by default. Drag the slider to the left on the slider bar and change this value
    to **5**.

5.  Under the **Mark as spam** section, update the following settings:

    -   Empty messages: **Off**

    -   Embedded tags in HTML: **On**

    -   JavaScript or VBScript in HTML: **On**

    -   SPF record hard fail: **On**

    -   Sender ID filtering hard fail: **On**

    **Note:** These next two settings allow you to automatically tag messages
        as spam when they originate from countries/regions that are to be
        avoided or distrusted, as well as messages written in specific languages.
   
    -   Contains specific languages: **On**  

        If you plan to use this setting, you should already know the languages that you want to filter. In the
        blank field that appears below the **Contains specific languages**
        field, enter the first letter of a language that you want to filter.
        This will display all languages that start with that letter (as well as
        any languages that contain that letter within the name of the language).
                
        Enter a letter and then select a language with the letter in it that you
        want to filter. Repeat this step for a couple of languages. 

	**Important:** We obviously can't implement this feature in this lab, but this exercise enables to see where this setting can be implemented (which is the same for the next setting as well). 

    -   From these countries: **On**

	Again, if you plan to use this setting, you should already know the countries/regions that you want to filter. In the
        blank field that appears below the **From these countries** field, enter
        the first letter of a country/region that you want to filter. This will display
        all countries/regions that start with that letter (as well as any countries/regions that
        contain that letter within the name of the country/region).

	Enter a letter and then select a country/region with the letter in it that you
        want to filter. Repeat this step for a couple of countries/regions.

6.  Select **Save**.

7.  This returns you to the **Anti-spam inbound policy (Default)** pane. Scroll
    to the bottom of the **Actions** section and select the **Edit actions**
    link. ‎

8.  In the **Actions** pane, scroll to the top of the pane (if necessary) and update the following settings:

    -   Spam: **Move message to Junk Email folder**

    -   High confidence spam: **Prepend subject line with text**

    -   Phishing email: **Quarantine message**

    -   High confidence phishing email: **Quarantine message**

    -   Bulk: **Move message to Junk Email folder**

    -   Retain spam in quarantine for this many days: **10**

    -   Prepend subject line with this text: enter **WARNING: This message contains potential spam!**

9.  Select **Save** to update the settings, and then select **Close** to close
    the **Anti-spam inbound policy (Default)** pane.

10. In your Edge browser, close the **Microsoft 365 Defender** tab (the tab name in your browser is **Anti-spam policies - Microsoft 365 security**), but
    leave all other tabs open.

### Task 10 – Manage Mail Flow Rules

After Holly reviewed the messaging environment at Adatum Corporation, she
discovered that Adatum’s current mail flow policy is to simply wait until
messages are delivered to mailboxes before being acted upon by Inbox rules in
Outlook and Outlook on the web. Holly realized she could provide a more
efficient and secure environment if she created a set of mail flow rules that
identify and act on messages that are in-transit through Adatum's Exchange Online
organization.

Holly has discovered that mail flow rules contain a richer set of conditions,
exceptions, and actions, all of which will provide her with the flexibility to
implement many types of messaging policies for Adatum. She is eager to put this
to the test regarding a significant issue currently affecting Adatum’s messaging
environment - users who send extremely large email messages. She has decided
that her first task will be to create a mail flow rule that restricts email
size.

1.  On LON-CL1, in the **Microsoft 365 admin center**, select **Exchange** in the navigation pane. This opens the Exchange admin center for Exchange Online.

2.  In the **Exchange admin center** navigation pane, select
    **Mail flow** to expand this group. Under this group, select **Rules**.

3.  In this **Rules** page, you can create rules based on a variety of options to
    protect against emails being sent from Adatum users. You can also create custom rules to prevent or track
    messaging-related issues from recipients in your environment. For this lab, you will create an email size restriction rule. <br/>
    
    In the menu bar that appears over the list of mail flow rules (there are no rules at this point), select the
    **plus (+)** sign. In the menu that appears, select **Filter messages by
    size.**

4.  In the **new rule** window that appears, enter the following information.

    -   Name: **Email size restriction**

    -   Apply this rule if: **The message size is greater than or equal to...**

        -   To the right of this drop-down field, select **Enter text**.

        -   In the **specify size (KB)** window that appears, 512 appears by default. Change this value to **1024** and
            then select **OK**.

    -   Do the following: Select in this field, which displays a drop-down menu
        of options. Hover your mouse over **Block the message...**, and then in
        the drop-down menu that appears, select **Reject the message and include
        an explanation**.

        -   In the **specify rejection reason** window, enter the following
            text: **Your message exceeds the size limit. Please adjust the message size or compress the email content and send it as a zipped file.**

        -   Select **OK.**

    -   Under **Choose a mode for this rule** setting, select **Enforce.**

5.  Select **Save**. This may take a minute or so to create the new rule.

6.  Leave your Edge browser open as well as all the tabs.

### Task 11 – Validate Accepted Domains

A domain that’s added to an organization’s on-premises environment is called an
accepted, or custom domain. You can create mailboxes with accepted domains to
receive and send email. In Lab 1, you created a custom, on-premises domain for Adatum Corporation
based on the unique UPN name assigned to your tenant
(xxxUPNxxx.xxxCustomDomainxxx.xxx, where xxxUPNxxx is your unique UPN Name) and
the custom domain name provided by your lab hosting provider
(xxxCustomDomainxxx.xxx). You also created the three DNS records that are required to connect this custom, on-premises domain with Adatum's Microsoft Exchange Online service. This accepted domain was automatically flagged as Adatum's default domain.

In this task, you will use the Exchange admin center (for Exchange Online) to view this accepted domain
and configure its domain type. Each domain can be
changed to either authoritative (which accepts all inbound or outbound mail) or
internal relay (which only accepts internal email). By default, all domains
should be set to authoritative. You want to ensure the domain
type for your custom, on-premises domain is set to authoritative.

1.  The **Exchange admin center** should still be displayed following the
    previous task. In the **Mail flow** group in the navigation pane,
    select **Accepted domains.**

2.  On the **Accepted domains** page, see Adatum’s two domains – its custom
    on-premises domain **(xxxUPNxxx.xxxCustomDomainxxx.xxx)** that you added in Lab
    1, and its Microsoft 365 cloud domain **(xxxxxZZZZZZ.onmicrosoft.com)**.

3.  You can see from this display that the domain type for each domain is
    already set to **Authoritative,** so you don’t need to make any changes
    here.

4.  However, let’s assume that you set the domain type to **Internal Relay**
    when you initially created the custom **xxxUPNxxx.xxxCustomDomainxxx.xxx**
    domain. If you wanted to change it now to **Authoritative,** you would
    perform the following steps (you can perform the first step to see the
    window and the corresponding options, but the domain is already set to
    Authoritative, so you can’t make this change). <br/>

    -   Select this domain in the list, which opens a detail pane for the domain
        on the right-side of the screen.

    -   In the detail pane for this domain, under **This accepted domain is**
        section, you would select the **Authoritative** option and then select
        **Save**.   
        
        However, since this domain is already set to **Authoritative** and you
        did not make any changes, select the **X** in the upper-right corner to close this pane.

5.  Close the **Exchange admin center** tab in your Edge browser. This will
    return you to the **Microsoft 365 admin center** tab. 

6. On the **Microsoft 365 admin center**, under the **Settings** group in the navigation pane, select **Domains**. 

7. On the **Domains** page, select the custom **xxxUPNxxx.xxxCustomDomainxxx.xxx** that you created in Lab 1, which is flagged as the default domain.

8. On the **xxxUPNxxx.xxxCustomDomainxxx.xxx** page, the **Overview** tab is displayed by default. Select the **DNS records** tab. This displays the three DNS records that you created in lab 1 that will enable this custom, on-premises domain to connect with Adatum's Microsoft Exchange Online service. 

9. Select the **MX** record to open its properties page. Note how the pane display the expected DNS record values and the actual DNS record values that you entered. Since the values are in sync, a message is displayed indicating the record is set up correctly for your domain in Azure. Select **Done**. If you select any of the other DNS records, you should see a similar result. 

9. You have now completed the validation of the custom, on-premises domain that you created in Lab 1. Leave your browser and all tabs open for the next lab exercise. 

### Proceed to Lab 3 - Exercise 2
