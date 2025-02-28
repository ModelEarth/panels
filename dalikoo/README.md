#Dalikoo New Hires webpart

[About New Hires webpart](https://dalikoo.com/new-hires-for-sharepoint/)

**Our problem with set-up:**  
The path to List in Sharepoint is not finding the data, and
The path to an Excel file is returning 400 and 404.

The Excel path we're using matches Dalikoo's:  
[How to obtain file path (URL) for a file in a SharePoint library](https://dalikoo.com/how-to-obtain-file-path-url-for-a-file-in-a-sharepoint-library/)

[Export an Excel table to SharePoint](https://support.microsoft.com/en-us/office/export-an-excel-table-to-sharepoint-974544f9-94bc-4aa8-9159-97282d256dab)  
Not sure how to get to Table Design  


[Copy format of list (dalikoo.com/sharepoint-list)](https://dalikoo.com/sharepoint-list)
After importing Excel to a list, add a column called UserName and choose type person. Manually populate by pasting each person's name to do a lookup (unless we find a means to automate).

Format for phone list conversion for List

	=LOWER(SUBSTITUTE(LEFT(E2,1) & F2 & "@web.org", " ", ""))
