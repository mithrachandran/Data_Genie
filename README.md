# Data_Genie
In this project, Power BI fetches the Monthly Sales Data for an organization "Data Genie" directly from Outlook without opening the email and loading and transforming the data, making an aesthetic dashboard, and sending it directly to the stakeholders.

To start the project, open Outlook, the home tab, rules, and create rules.
![sc1](https://github.com/mithrachandran/Data_Genie/assets/145925652/a9c3580d-a06f-4b3c-9e52-c6e3e8eb8d9c)

Select subject contains tab
Write the file name
Select “move item to folder”, and select the folder 
The name of the folder is “Monthly sales data”, click on the OK button
![sc3](https://github.com/mithrachandran/Data_Genie/assets/145925652/a552ac9f-408f-4487-b5ce-57f1ec4dbb5b)
A new folder appears
Click on the OK button
Pop up window appears asking whether to apply the rule right away- click yes

![sc4](https://github.com/mithrachandran/Data_Genie/assets/145925652/6f71e454-e68b-41ab-834d-f6b0502fe8fa)

![sc5](https://github.com/mithrachandran/Data_Genie/assets/145925652/1e9f7d47-0039-4f84-84c0-104440997207)

How to get the email attachments on Power BI without opening the email?

Click on the Get Data tab on Power BI UI.
On the search tab (connector) type "exchange" then select Microsoft Exchange Online and click connect
![sc7](https://github.com/mithrachandran/Data_Genie/assets/145925652/08d73386-6129-4ce4-9518-41de3c8d3d97)

A tab appears asking for the corporate email ID. Enter the corporate email address( only that will work), click ok
Click Microsoft account sign in, click connect
![sc13](https://github.com/mithrachandran/Data_Genie/assets/145925652/8fc4fe2e-829f-4927-8a70-0ab577d7197f)
Now all the data inside Outlook is in Power BI. Here I require only mail. select Mail and transform data.

![sc8](https://github.com/mithrachandran/Data_Genie/assets/145925652/cd8aa79a-a3b7-4d83-afca-ef960d046cc7)

Now all the folders of Outlook are loaded into the first column "Folder Path"
Click on the drop-down arrow of the folder path, and load more .click on the Folder Path and filter for the "Monthly_Sales_Data"
![sc9](https://github.com/mithrachandran/Data_Genie/assets/145925652/0b693949-cf9b-40cd-9078-71637f6ba12d)

On the right, we can find the column attachment. Select that column and remove other columns.
Now click on the expansion of attachment which shows details about the attachment of the email.

On the right, we can see the Attachment .content column, which has all the information about the attachment of the email.  Keep only that column and remove the other columns.

Add a custom column
Use csv. Document function to extract all the data from that column which are CSV files.

![sc18](https://github.com/mithrachandran/Data_Genie/assets/145925652/36156139-c05e-4402-b827-5e615a428e9e)

![sc22](https://github.com/mithrachandran/Data_Genie/assets/145925652/4e41d03a-641a-4b9c-8dac-e982ae590df8)
Keep the Custom column, remove the other column. Expand the table. All the data in the email attachment can be accessed here.

![sc24](https://github.com/mithrachandran/Data_Genie/assets/145925652/17e64bdb-77e7-4774-9d5a-555ce2fbfc09)

The dashboard is built and shared using Power BI Publish.
![sc25](https://github.com/mithrachandran/Data_Genie/assets/145925652/e149ff8b-d685-40c4-b78f-5607a70d8ec2)

This report can be sent to the stakeholders by adding new subscriptions so that the receiver will get regular updates weekly monthly etc.

In my workspace on the dataset, there is a settings tab where edit the credentials to give access to Power BI to access my email so that every time a new monthly sales report comes to the email it gets updated to the report automatically by data refresh.



