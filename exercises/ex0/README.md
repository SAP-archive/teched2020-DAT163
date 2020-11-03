# Objective 

As a Data Steward. you need to understand and gain insight into your data.  After profiling and reviewing the profiling results you will be able to add a glossary term to a column in your dataset as well as rate and comment on the dataset.  

In this exercise, you will upload datasets, profile the data, rate dataset, create a relationship with data and a glossary term


## Log Into SAP Data Intelligence

After completing these steps you will have logged into SAP Data Intellegence

1.	Open Chrome and go to (UPDATE: add URL)
<br>![](/exercises/ex0/images/LogOn_Default_00_05.png)

2.	Enter 'Default' for Tenant Name and click 'Proceed'
<br>![](/exercises/ex0/images/LogOn_Default_00_10.jpg)

3.	Enter 'Username_##', where ## is the Number you were assigned (UPDATE: username with correct usename and group number) for Tenant Name and 'Welcome01' for your Password and click 'Sign In'
<br>![](/exercises/ex0/images/LogOn_uname_pwd_00_20.jpg)

## Upload and publish datasets

After completing these steps you will have uploaded and published datasets in SAP Data Intellegence

4.	Click on 'Metadata Explorer'
<br>![](/exercises/ex0/images/DI_HomeScreen_00_30.png)

5.	Click on 'Browse Connections'
<br>![](/exercises/ex0/images/MM_Home_00_40.png)

5.	Click on the 'DI_DATA_LAKE' tile
<br>![](/exercises/ex0/images/BrowseConnection_DI_DATA_LAKE_00_50.png)

6.	Click on the 'shared' tile
<br>![](/exercises/ex0/images/BrowseConnection_shared_00_60.png)

6+. Upload a file, click on the 'Upload Files' icon on the toolbar
<br>![](/exercises/ex0/images/BrowseConnection_UploadFile_00_62.png)

6+. Click on the '+' in the upper right hand corner of the Upload Files pop-up window
<br>![](/exercises/ex0/images/BrowseConnection_UploadFilePopUp_00_64.png)

6+. Browse to Sample Data folder (UPDATE to correct directory) and select 'Customer_US.parquet' Click 'Open'
<br>![](/exercises/ex0/images/BrowseConnection_UploadCustomerFiles_00_65.png)

6+. Click on the '+' in the upper right hand corner of the Upload Files pop-up window
UPDATE Screen shot with no error
<br>![](/exercises/ex0/images/BrowseConnection_UploadedCustomer_00_66.png)

6+. Select 'Sales_data.csv' Click 'Open'
<br>![](/exercises/ex0/images/BrowseConnection_UploadCustomerFiles_00_65.png)

6+. Click on the '+' in the upper right hand corner of the Upload Files pop-up window
UPDATE Screen shot with no error
<br>![](/exercises/ex0/images/BrowseConnection_UploadedCustomer_00_66.png)

6+. Click 'Upload'
<br>![](/exercises/ex0/images/BrowseConnection_UploadedSales_00_67.png)

7.	Locate 'Customers_US2.parquet' file and drag the file to the right and drop in the right pane 'Drag and drop datasets and folders to publish'
<br>![](/exercises/ex0/images/BrowseConnection_CustomerFiles_00_75.png)

8.	Locate 'Sales_data.csv' file and drag and drop the file to the righ
<br>![](/exercises/ex0/images/BrowseConnection_DragSales_00_75.png)

9.	Enter 'TechEd_DAT163_##' in the Name parameter and "TechEd_DAT163 Group ## in the Description parameter
 Note: where ## is the number assigned to you 
<br>![](/exercises/ex0/images/BrowseConnection_Name_Desc_00_90.png)

9.	Click Publish
<br>![](/exercises/ex0/images/BrowseConnection_Name_Desc_00_90.png)

## Profile and rate the dataset

After completing these steps you will have profiled, viewed the fact sheet, and rate the dataset in SAP Data Intellegence

10. Click the drop down 'Data Intelligence Metadata Explorer' at the top and select 'Browse Catalog
<br>![](/exercises/ex0/images/MM_DropDownHome_00_10.png)

11. Click on the 'DI_DATA_LAKE' tile
<br>![](/exercises/ex0/images/BrowseCatalog_DI_DATA_LAKE_00_20.png)

12.	Click on the 'shared' tile
<br>![](/exercises/ex0/images/BrowseCatalog_shared_00_30.png)

UPDATE: May need to click on a TechEd folder?

14. Locate and hover over Customers_US2.parquet(##) file and select 'Start Profiling'
<br>![](/exercises/ex0/images/DataCatalog_SalesProfile_00_40.png)

14. Click 'Yes' to confirm profiling
<br>![](/exercises/ex0/images/BrowseCatalog_YesProfile_00_50.png)

14. Locate and hover over Sales_data.csv (##) file and select 'Start Profiling'
<br>![](/exercises/ex0/images/DataCatalog_SalesProfile_00_50.png)

14. Click 'Yes' to confirm profiling
<br>![](/exercises/ex0/images/BrowseCatalog_YesProfile_00_55.png)

14. Locate and hover over Customers_US2.parquet(##) file and select the 'glasses' to View Fact Sheet
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheetGlasses_00_40.png)

15. View Customer Fact Sheet
Click on Data Preview
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheet_00_40.png)

16. Click on 'View Tag Tree' 
<br>![](/exercises/ex0/imagesDataCatalog_CustomerFactSheetViewTree_00_40.png)

17. Note a few tags automatically added based on the data
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheetTag_00_40.png)

18. Click on 'Conversation Bubble' icons next to the 5 stars
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheetRatingExisting_00_40.png)

19 Click 'Close' after reviewing comment
<br>![](/exercises/ex0/images/DataCatalog_CloseComment_00_40.png)

20. Click on the 5 stars to add your own comment
<br>![](/exercises/ex0/images/DataCatalog_AddComment_00_40.png)

20. Click on the 3 stars and add 'Also does not have Name split into First Name and Last Name per our organizational rules' to the Comments
<br>![](/exercises/ex0/images/DataCatalog_AddCommentSave_00_40.png)

22. Click 'OK'
<br>![](/exercises/ex0/images/DataCatalog_AddCommentSave_00_40.png)

## Search, add, and associate a glossary term

After completing these steps you will have search the glossary, added a glossary term, and associated the term with a column in SAP Data Intellegence

23. Click the drop down 'Data Intelligence Metadata Explorer' at the top and select 'Glossary' on the left hand side
<br>![](/exercises/ex0/images/MM_DropDownHome_00_10.png)

24. Click on 'View Business Glossaries'
<br>![](/exercises/ex0/images/Glossary_MainMenu_00_10.png)

25. In the Search business glossary on the right enter 'address' and then click on the magnifying glass or press Enter
<br>![](/exercises/ex0/images/Glossary_AddressSearch_00_20.png)

25. The term 'Address' is not found
<br>![](/exercises/ex0/images/Glossary_TermNotFound_00_30.png)

26. Click on the '+' on the right to Create a term
<br>![](/exercises/ex0/images/Glossary_AddTerm_00_40.png)

27. For Name enter 'Address'
<br>![](/exercises/ex0/images/Glossary_Address_00_50.png)

27. For Definition enter 'A collection of information, used to give the location of a building, apartment, or other structure containing street names, house number, city, region, postal code and country.’ 
<br>![](/exercises/ex0/images/Glossary_AddressDefiition_00_60.png)

28. For Keywords type 'street' press the Enter key
                 type 'city' press the Enter key
                 type 'state' press the Enter key
                 type 'zip code' press the Enter key
<br>![](/exercises/ex0/images/Glossary_AddressKeywords_00_70.png)

29. For Synonyms enter 'addr' 
<br>![](/exercises/ex0/images/Glossary_AddressSaved_00_80.png)

30. Click on 'Approve*'
<br>![](/exercises/ex0/images/Glossary_Approve_00_90.png)

31. Enter <Today's Date> for Approve Date
    Enter 'James Lee' for Approver
    Click 'Save'
<br>![](/exercises/ex0/images/Glossary_ApproveSave_00_90.png)

32. Click on 'Relationships'
<br>![](/exercises/ex0/images/Glossary_Relationship_00_100.png)

33. Click 'Edit' in the bottom right hand corner
<br>![](/exercises/ex0/images/Glossary_RelationshipsEdit_00_10.png)

34. Click 'Edit Related Objects' 
<br>![](/exercises/ex0/images/Glossary_RelationshipsMain_00_10.png)

35. Click 'Datasets/Columns' 
<br>![](/exercises/ex0/images/Glossary_RelationshipsEditObjects_00_10.png)

36. Expand 'DI_DATA_LAKE' 
    Expand 'shared' 
    Expand 'TechEd163_##' (where ## is the Number assigned to you)
    Expand 'Customers_US2.parquet' in the tree structure
<br>![](/exercises/ex0/images/Glossary_RelationshipsExpandTree_00_10.png)

37. Select / Check 'Address1', 'Address2, and 'Address3'
<br>![](/exercises/ex0/images/Glossary_RelationshipsColumns_00_10.png)

38.  Click 'Save Related Objects' located in the bottom right hand corner.  You can now see that you have created a relationship between 'Address1', 'Address2', and 'Address3' to the glossary term 'Address'
<br>![](/exercises/ex0/images/Glossary_RelationshipsSavedAssociationLineage_00_10.png)

10. Click the drop down 'Data Intelligence Metadata Explorer' at the top and select 'Browse Catalog
<br>![](/exercises/ex0/images/MM_DropDownHome_00_10.png)

11. Click on the 'DI_DATA_LAKE' tile
<br>![](/exercises/ex0/images/BrowseCatalog_DI_DATA_LAKE_00_20.png)

12.	Click on the 'shared' tile
<br>![](/exercises/ex0/images/BrowseCatalog_shared_00_30.png)

UPDATE: May need to click on a TechEd folder and add screen shot?

14. Click on Customers_US2.parquet(##) file on the left side scroll down to Glossary and see the associated term 'Add 
<br>![](/exercises/ex0/images/Glossary_Catalog_Relationships_00_10.png)

## Summary

Now that you have completed your work around the data catalog by uploading datasets, profiling datasets, rating and commenting on datasets, and using the glossary, lets continue by creating and using validation and quality rules. 
Continue to - [Exercise 2 - Rule Creation, Testing Rule, Rulebooks, and Data Quality Dashboards](../ex1/README.md)
