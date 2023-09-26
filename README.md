# Data_Genie
In this project, Power BI fetches the Monthly Sales Data for an organization "Data Genie" directly from Outlook without opening the email and loading and transforming the data, making an aesthetic dashboard, and sending it directly to the stakeholders.

To start the project, open Outlook, the home tab, rules, and create rules.


![Image](https://github.com/users/mithrachandran/projects/1/assets/145925652/aba2678c-ffb9-4ae2-a439-e9e9a2e8b12b)
*********************************************************
Select subject contains tab
Write the file name
Select “move item to folder”, and select the folder 
The name of the folder is “Monthly sales data”, click on the OK button


![Image](https://github.com/users/mithrachandran/projects/1/assets/145925652/6fb098bf-e407-4180-a1e6-4c2043e419de)

************************************************************
A new folder appears
Click on the OK button
Pop up window appears asking whether to apply the rule right away- click yes


![Image](https://github.com/users/mithrachandran/projects/1/assets/145925652/edbe25df-89d4-4c2c-a1b8-003b54d70cb5)
![Image](https://github.com/users/mithrachandran/projects/1/assets/145925652/51b74c08-f334-43f3-ad51-b3cc44ab089e)

************************************************************
How to get the email attachments on Power BI without opening the email?

Click on the Get Data tab on Power BI UI.
On the search tab (connector) type "exchange" then select Microsoft Exchange Online and click connect


![Image](https://github.com/users/mithrachandran/projects/1/assets/145925652/637fcff9-ed8f-4062-9d87-c296b2886fca)

A tab appears asking for the corporate email ID. Enter the corporate email address( only that will work), click ok
Click Microsoft account sign in, click connect
![image](https://github.com/mithrachandran/Data_Genie/assets/145925652/74913690-80a5-46ef-8085-a6fcec16380d)

 
Now all the data inside Outlook is in Power BI. Here I require only mail. select Mail and transform data.


![Image](https://github.com/users/mithrachandran/projects/1/assets/145925652/8c08ba5f-aac5-4483-b755-174a7ed2f241)

Now all the folders of Outlook are loaded into the first column "Folder Path"
Click on the drop-down arrow of the folder path, and load more .click on the Folder Path and filter for the "Monthly_Sales_Data"


![Image](https://github.com/users/mithrachandran/projects/1/assets/145925652/c8b840d5-27b6-4aaf-b5b5-9dfba2d593bb)



On the right, we can find the column attachment. Select that column and remove other columns.
Now click on the expansion of attachment which shows details about the attachment of the email.

On the right, we can see the Attachment .content column, which has all the information about the attachment of the email.  Keep only that column and remove the other columns.

Add a custom column
Use csv. Document function to extract all the data from that column which are CSV files.

![Image](https://github.com/users/mithrachandran/projects/1/assets/145925652/6ef17ead-4cc6-4d8c-8d7c-0536dc7e8fc9)


![Image](https://github.com/users/mithrachandran/projects/1/assets/145925652/ea7df691-6eeb-4c71-81dd-672065ab8a9a)

Keep the Custom column, remove the other column. Expand the table. All the data in the email attachment can be accessed here.

![Image](https://github.com/users/mithrachandran/projects/1/assets/145925652/31bc9185-1ba6-48e2-aac7-91c1ce4d28f6)

The dashboard is built and shared using Power BI Publish.


![Image](https://github.com/users/mithrachandran/projects/1/assets/145925652/34dafa6c-d5f9-4334-88c1-ce961ce18a2f)

This report can be sent to the stakeholders by adding new subscriptions so that the receiver will get regular updates weekly monthly etc.

In my workspace on the dataset, there is a settings tab where edit the credentials to give access to Power BI to access my email so that every time a new monthly sales report comes to the email it gets updated to the report automatically by data refresh.
