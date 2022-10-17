# Learning Path 4 - Lab 3 - Exercise 2 - Review Key Features of SharePoint Online

Adatum's CTO has heard a lot about Microsoft SharePoint Online and is interested in implementing it at Adatum. However, security is of the utmost concern to the CTO, who is worried whether new sites created within the company can be kept secure. The CTO has tasked Holly with reviewing some of the basic administrative functions in SharePoint Online to determine whether it can meet their security requirements.

### Task 1 – Site Management

A team site includes a group of related web pages, a default document library for files, lists for data management, and web parts that can be customized to meet your collaboration needs. Holly is excited about the possibility of using team sites in SharePoint Online to improve collaboration between team members when working on specific projects. As part of Adatum's pilot project, Holly wants to create a team site for the IT department so that IT personnel can work on projects and share information from anywhere and on any device. 

1. You should still be logged into LON-DC1 as **Administrator** and password **Pa55w.rd**; if not, then do so now.

2. You should still have Microsoft Edge and the **Microsoft 365 admin center** open from the prior lab, and you should be logged in as Holly Dickson. If so, proceed to the next step; otherwise, open Edge, navigate to **https://portal.office.com/**, log in as **Holly@xxxxxZZZZZZ.onmicrosoft.com** (where xxxxxZZZZZZ is the tenant prefix provided by your lab hosting provider) and **User.pw1**, and then on the **Microsoft Office Home** page, navigate to the **Microsoft 365 admin center**.

3. In the **Microsoft 365 admin center**, select **Show all** in the navigation pane (if necessary), then scroll down to **Admin centers** and select **SharePoint.** This will open the SharePoint admin center.

4. In the **SharePoint admin center** navigation pane, select **Sites** and then select **Active sites.** 

5. In the **Active sites** window, select the **+Create** option on the menu bar.   

6.  Depending on the team or company need, there are several templates that can be used when creating a new site. For the purposes of this lab, in the **Create a site** window, select the **Team site** tile.

7. In the **Create a team site** window, enter the following information.

	- Site name: **IT Services**

	- Group email address: this is the alias for the group email address. As you typed in **IT Services** in the **Site name** field, the same text automatically prefilled in this field, although the blank space was removed so that it appears as one word (ITServices). Do not change this default value.

	- Site address: As you typed in **IT Services** in the **Site name** field, the same text automatically prefilled in this field, although the blank space was removed so that it appears as one word (ITServices). Do not change this default value.

	- Group owner: type **Holly**. If Holly Dickson's name does not appear, select **Search directory**. In the window that appears displaying the users whose first name starts with Holly, select **Holly Dickson**.  

	- Select a language: Leave this as **English**

	- Select **Advanced settings** to expand this section and then enter the following information:

		- Privacy settings: Given the confidential nature of much of the IT department's information, select **Private – only members can access this site**

		- Time zone: since this group is in Adatum’s Redmond, WA location, select **Pacific Time (US and Canada)**

		- Site Description: **Team site for the IT department** 

8. Select **Next**.

9. In the **Add site owners and members** window, in the **Add members** field, enter **Patti**. As you enter Patti, a window appears listing users whose first name starts with Patti. Select **Patti Fernandez**. 

10. Repeat the previous step for **Nestor Wilke** and then **Diego Siciliani**.

11. You now want to make Diego an owner of the group, along with Holly. The **Add site owners and members** window currently displays Patti, Nestor, and Diego as members of the group. Below **Diego Siciliani**, select the **Member** drop-down arrow. In the drop-down menu that appears, select **Owner**. This changes Diego from a group member to a group owner.

12. Select **Finish**.
 
13. The **IT Services** site should now appear in the list of **Active sites** (it may take a minute or so to appear in the list). Scroll the horizontal scroll bar to the right to view all the information for the IT Services site and all the other sites in the list. When you've finished, scroll the horizontal scroll bar all the way back to the left.

14. You’re now going to test the process of deleting a team site and then restoring it. In the list of **Active sites**, hover your mouse to the left of the **IT Services** site name, which should display a circle. Select this circle (do not select the IT Services site name, as this will open a properties window for the site). 

	**Tip:** Selecting the circle to the left of an item in a display view enables you to perform any of the tasks on the menu bar for the selected item. Some tasks require you to select multiple items, in which case the task you perform in the menu bar will be performed on all the selected items. 
	
15. In the menu bar at the top of the page, select **Delete**. 

16. In the **Delete Microsoft 365 Group** pop-up window that appears, select the **Delete the group “IT Services” and all its resources** check box and then select **Delete.** Note that the IT Services site disappears from the **Active sites** list. 

17. In the **SharePoint admin site** navigation pane, under the **Sites** group, select **Deleted sites.** Note how the IT Services site that you just deleted appears in the list of deleted sites (it may take a minute or so to appear in the list). 

18. In the **Deleted sites** window, select the circle to the left of the **IT Services** site name (do not select the IT Services site name).

19. In the menu bar at the top of the page, select **Restore**.

20. In the **Restore Microsoft 365 Group** pop-up window that appears, select **Restore**. Note that the IT Services site disappears from the **Deleted sites** list. 

21. In the **SharePoint admin site** navigation pane, under the **Sites** group, select **Active sites.** The IT Services site should once again appear in the **Active sites** list. 

22. In the **Active sites** list, select the circle to the left of the **IT Services** site name to highlight this site. Scroll the horizontal scroll bar to the right to verify that all the information for the IT Services site has been restored. 

23. Remain in the SharePoint admin center for the next task.

 
### Task 2 – Hierarchical Permissions

SharePoint Online uses hierarchical permissions to set authorization and access of sites. In other words, when a site is created (known as the parent site) any sites that are later created under that site (known as children sites) will, by default, inherit the main site permissions of the parent site. Since you just created a team site for IT Services, you now plan to configure site permissions to meet the IT team's security requirements.

In this task, you will create the following hierarchical permission structure for Adatum:

- When you created the IT Services team site in the prior task, you assigned Diego Siciliani as group owner of the site, and you assigned Patti Fernandez and Nestor Wilke as group members for the site. In doing so, the default team site permission levels were assigned to Diego, Patti, and Nestor. Diego was assigned Full Control permission (as site owner), and Patti and Nestor were assigned Edit permissions (as site members). In this task, you will verify these default team site permission levels were automatically assigned to Diego, Patti, and Nestor.

- You want to assign a different set of permissions for a different group of users, so you will follow best practices by creating a group of users and assigning the group a custom permission level (as opposed to assigning custom permissions to each individual user). In this case, you will create a new **Information Technology** group. You will then assign Isaiah Langer and Joni Sherman to this group, and will you assign the group Full Control permissions. 

- You will then create a permission level titled **Designer**, which will be used for Adatum’s web specialists who will design SharePoint sites upon request. They need to be assigned permission levels that provide complete editing and administrative capabilities. Although you won't do this in this lab, you can later create a group for your web designers and assign that group this Designer permission level.  

1. In the **SharePoint admin center**, you should still be displaying **Active sites**.

2. In the list of active sites, for the **IT Services** site that you created in the prior task, select the site's URL value (**.../sites/ITServices**) that appears under the **URL** column. 

3. A new tab will open in your Edge browser that displays the **IT Services** site. If a **Start designing your site** dialog box appears, select **Maybe later**.

4. In the upper right-hand corner of the **IT Services** site (to the left of the circle containing Holly Dickson's initials), select the **gear (Settings)** icon. In the **Settings** pane that appears, select **Site permissions.**

5. At the bottom of the **Permissions** pane that appears, select **Advanced permissions settings**, which opens a new **Permissions: IT Services** tab in your Edge browser.

6. In the ribbon that appears at the top of the screen, two tabs are available - a **BROWSE** tab and a **PERMISSIONS** tab, the latter of which is displayed by default. <br/>

	Select the **BROWSE** tab and note how the Permissions ribbon disappears. This also reveals the name of this page, which is **Site Settings > Permissions**.

7. Select the **PERMISSIONS** tab, which displays the Permissions ribbon. In the ribbon, under the **Check** section, select **Check Permissions.**  <br/>

	**Note:** This option enables you to check access permissions for users and groups. In this case, you will check the permissions that were assigned to Holly Dickson. In the prior task, you assigned Holly as an owner of the IT Services site. The following steps will enable you to check what default team site permissions were assigned in this role. 

8. In the **IT Services: Check Permissions** dialog box that appears, in the **User/Group** field, type **Holly**. As you type Holly, a window appears listing users whose first name starts with Holly. Select **Holly Dickson** and then select **Check now**. Since Holly is an owner of this site, this confirms that she was automatically assigned **Full Control** permissions through the **IT Services Owners** group.

9. In the **User/Group** field, select the **X** next to Holly’s name to remove it from the field. In the **User/Group** field, type **Nestor**. As you type Nestor, a window appears listing users whose first name starts with Nestor. Select **Nestor Wilke** and then select **Check now.** Since Nestor is a member of this site, the dialog box confirms that he was automatically assigned **Edit** permissions through the **IT Services Members** group.

	Repeat this step for Diego Siciliani and Patti Fernandez. As a site owner, Diego should have **Full Control** permissions, just like Holly. As a site member, Patti should have **Edit** permissions, just like Nestor. 
	
19. Repeat the prior step and check the permission for **Alex Wilber**, who is not a site member. You will see that Alex's permission level is set to **None**, which means he does not have permission to access or update the site since he has not been assigned as a site member or site owner.

11. In the **IT Services: Check Permissions** window, select **Close.**

12. You are now back in the **Permissions: IT Services** tab in your browser. You have been asked to create a new group of users and assign them permission to access the IT Services site. In the ribbon that appears at the top of the page, under the **Grant** section, select **Create Group.**  

	‎**Best Practice:** As a best practice, you should use **Groups** to assign access permissions rather than assigning access to individual user accounts for two important reasons: 1) Assigning individual users access to a site makes it difficult to track user access when the user leaves your organization, and 2) Individual user permissions can override security group permissions.

13. In the **People and Groups > Create Group** window, enter the following information:   

	- Name: **Information Technology** (Select the X in the dialog box that appears below this field to close it)

	- About me: **This group is used for members of the IT staff**

	- Group owner: If Holly Dickson appears as the owner, select the **X** to the right of her name to remove her, and then enter **MOD**. As you type MOD, a window appears listing users whose first name starts with MOD. Select **MOD Administrator**.  
	
		‎**Best Practice:** When you create groups make sure the group owner is either a generic Administrator account (such as the MOD Administrator) or an Administrator group. Giving ownership of groups to individuals can cause editing issues because only the owners can make changes to groups.

	- Group Settings:

		- Who can view the membership of the group: **Group Members**

		- Who can edit the membership of the Group: **Group Owner**

		- Allow requests to join/leave this Group: **Yes**

		- Auto-accept requests: **No**

		- Send membership requests to the following e-mail address: If Holly Dickson’s email appears, replace her email with the MOD Administrator's email, which is **admin@xxxxxZZZZZZ.onmicrosoft.com** (simply replace **holly** with **admin** in the email address). If this field is blank, enter **admin@xxxxxZZZZZZ.onmicrosoft.com**.

		- Choose the permission level group members get on this site: **Full Control – Has full control**

14. Select the **Create** button that appears at the  bottom of the screen. 

15. This displays the **Information Technology** group information. The users displayed in the list are the members of this group. Since Holly Dickson created the group, she is listed as the sole member.

16. In the menu bar that appears above the user list, select the drop-down arrow that appears next to **New**, and then in the drop-down menu, select **Add users**.

17. In the **Share ‘IT Services’** window, the **Invite people** tab is selected in the left-hand pane by default. In the **Enter names or email addresses** field, enter **Isaiah**. As you type Isaiah, a window appears listing users whose first name starts with Isaiah. Select **Isaiah Langer**. 

	Repeat this step for **Joni Sherman** (type **Joni** next to Isaiah Langer's name in the **Enter names or email addresses** field).

18. Below the personal message field, select **SHOW OPTIONS.**

19. Uncheck (clear) the **Send an email invitation** check box.

20. Select **Share** to share the IT Services site with the members of this Information Technology group.

21. In the **People and Groups > Information Technology** window that appears, the members of the group (Holly, Isaiah, and Joni) should be displayed.

22. Close this **Peoples and Groups** tab in your Edge browser. This will return you to the **SharePoint admin center** and the **Active sites** list, with the **IT Services** pane displayed on the right-hand side. 

23. In the **IT Services** pane, select the URL (**.../sites/ITServices**) that is displayed under **URL.** 

24. A new tab will open in your Edge browser that displays the **IT Services** site.

25. In the upper right-hand corner of the **IT Services** site, select the **gear (Settings)** icon (it may take a minute or so to appear).

26. In the **Settings** pane that appears, select **Site permissions.**

27. At the bottom of the **Permissions** pane, select **Advanced permissions settings**, which opens the **Permissions: IT Services** tab for the IT Services site.

28. On the ribbon that appears at the top of the page, under the **Manage** section, select **Permission Levels**.  

	‎**Note:** This option enables you to customize permission levels to better fit your organization.

29. In the **Permission Levels** window, in the menu bar at the top of the page, select **Add a Permission Level.**

30. You want to create a permission level for your team’s web specialists who will be designing SharePoint sites upon request. Adatum's CTO wants them to be assigned permission levels that provide complete editing and administrative capabilities. In the window that appears, enter the following information:

	- Name: **Designer** (Select the X in the dialog box that appears below this field to close it)
	
	- Description: **This level restricts the level of use for web designers**

	- List Permissions – select the following permission levels:

		- **Add Items** (which automatically selects the View Items, Browse Directories, View Pages, and Open permissions)

		- **Edit Items**

		- **Delete Items**

		- **Open Items**

		- **View Versions**

	- Site Permissions – select the following permission levels:

		- **Create Subsites** (which automatically selects the Browse User Information permission)

		- **Add and Customize Pages** (which automatically selects the Browse Directories permission)

		- **Apply Themes and Borders**

		- **Apply Style Sheets**

		- **Enumerate Permissions** 

		- **Use Remote Interfaces**

		- **Use Client Integration Features**

31. Select the **Create** button at the bottom of the page to save your changes.

32. The **Permission Levels** window now displays the **Designer** permission level that you just added.

33. In your Edge browser, close the **Permission Levels** tab. Leave the **SharePoint admin center** tab open as you will use it in the next lab exercise.


# Proceed to Lab 3 - Exercise 3
