# Learning Path 4 - Lab 3 - Exercise 5 - Review the Power Platform Admin Center

As Adatum begins its transition to Microsoft 365 as its hosted cloud solution, they want to use this opportunity to examine Microsoft’s Power Platform functionality. In your role as Holly Dickson, Adatum’s Enterprise Administrator, you have been asked to expand your Microsoft 365 pilot project to include Microsoft’s Power Platform. Therefore, your first task towards that goal is to familiarize yourself with the Power Platform admin center, which provides a unified portal for administrators to manage environments and settings for Power Apps, Power Automate, and Power BI. 

### Task 1 – Review the Power Platform Admin Center

In your role as Holly Dickson, you want to review the Power Platform admin center, which is the go-to destination for administrators who create, manage, and support their Microsoft Power Platform environments. 

1. Switch to **LON-DC1**, where you should still be logged in as **ADATUM\Administrator** and password **Pa55w.rd**; if not, then do so now.

2. On **LON-DC1**, you should still have your Microsoft Edge browser and the **Microsoft 365 admin center** open from the prior lab in which you were logged in as Holly Dickson. If so, proceed to the next step; otherwise, open Microsoft Edge, navigate to **https://portal.office.com/**, log in as **Holly@xxxxxZZZZZZ.onmicrosoft.com** (where xxxxxZZZZZZ is the tenant prefix provided by your lab hosting provider) and **Pa55w.rd**, and then in the **Microsoft 365 Home** page, navigate to the **Microsoft 365 admin center**.

3. In your Edge browser, close all tabs except for the **Microsoft Office Home** tab and the **Microsoft 365 admin center** tab. Open a new tab in your Edge browser and enter the following URL in the address bar: **https://make.powerapps.com/home** 

4. This opens the **PowerApps** studio. In the **Welcome to Power Apps** window, select **Get started**.

5. In the Contact information window, Holly's email address and country should be filled in. If the Phone number field is blank, enter **425-555-1234**. Select **Submit**.

6. On the **Make your job easier** window, select **Skip**.

7. On the **Power Apps** portal, select the **gear (Settings)** icon on the top right corner of the screen. In the **Settings** pane that appears, select **Admin center**. This opens a new tab that displays the **Power Platform admin center.** 

8. In the **Welcome to the Power Platform admin center** window, select the **X** in the upper right-hand corner to close it.

9. In the **Power Platform admin center**, select **Environments** in the left-hand navigation pane. 

10. On the **Environments** page, note how there is only one environment - the **Adatum Corporation (default)** environment. Select the **Adatum Corporation (default)** environment and review the information available for this environment. 

10. In the navigation pane at the top of the screen (**Environments > Adatum (default))**, select **Environments** to return back to the **Environments** page.

11. You have decided to create a new environment. On the menu bar at the top of the screen, select **+New** to create a new environment.

12. In the **New environment** pane that appears, enter the following information:

	- Name: **Adatum-Test**

	- Region: **United States - Default**

	- Type: **Sandbox**

	-  Create a database for this environment: **No**

	-  Pay-as-you-go with Azure: **No**

13. Select **Save.** <br/>

	**Note:** Trying to save this new environment record will result in an error message at the top of the window. This message indicates you need at least 1 Gb of database capacity, which is not available in your VM lab environment. 

14. Select **Cancel** to close the **New environment** window. 

15. An organization's data is critical to its success. Its data needs to be readily available for decision-making, but the data needs to be protected so that it isn't shared with audiences who shouldn't have access to it. To protect this data, you can use Power Apps to create and enforce data loss prevention (DLP) policies that define the consumer connectors that specific business data can be shared with. For example, an organization that uses Power Apps may not want the business data that's stored in SharePoint to be automatically published to its Twitter feed. <br/>

	You can create DLP policies for the data used within the Power Platform module. In the next several steps, you'll walk through the New Policy wizard to see what information is captured in a DLP policy. You won't actually create a policy, but you'll experience the process and see what information makes up a Power Platform DLP policy. <br/>

	In the **Power Platform admin center**, select **Policies** in the left-hand navigation pane, and then select **Data policies**.

16. On the **Data policies** page, select **+New Policy** that appears at the top of the page. This initiates the New Policy wizard.

17. On the **Name your policy** page, enter **Test** in the policy name field, and then select **Next**.

18. On the **Assign connectors** page, the **Non-business** tab is displayed by default. Note there are 821 non-business connectors at the time of this writing. These connectors are for non-sensitive data.

19. Select the **Business** tab. This tab displays existing connectors (there are none) for sensitive data. 

20. Select **Next**.

21. On the **Custom connector patterns** page, you can create a list of rules to limit access to custom connectors (in order of priority). Select **Next**.

22. On the **Define scope** page, you can define the environments that will be added to this policy. Do NOT select **Next**. Instead, select **Cancel** to cancel out of the New Policy wizard.

23. Explore other areas of the **Power Platform admin center**, as desired. 

24. When you are finished, close the **Power Platform admin center** tab in your browser.

25. In your browser, leave the **Power Apps** tab open for the next lab exercise.

 

# Proceed to Lab 3 - Exercise 6
