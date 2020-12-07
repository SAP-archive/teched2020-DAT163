# Objective 

As a Data Steward, you need to understand and gain insight into your data.  After profiling and reviewing the profiling results you will be able to add a glossary term to a column in your dataset as well as provide a rating and comment on the dataset.  

In this exercise, you will upload datasets, profile the data, rate dataset, create a relationship with data and a glossary term

## Log Into SAP Data Intelligence

After completing these steps you will have logged into SAP Data Intellegence

1.	Open Chrome and go SAP Data Intelligence url you were provided
<br>![](/exercises/ex0/images/LogOn_Default_00_05.png)

2.	Enter 'Default' for Tenant Name and click 'Proceed'
<br>![](/exercises/ex0/images/LogOn_Default_00_10.jpg)

3.	Enter the Username that was assigned to you (e.g. 'TA#'), for Tenant Name 
<br>Note: where # is the number assigned to you
<br> Enter the Password that was assigned to you, for your Password 
<br> Click 'Sign In'
<br>![](/exercises/ex0/images/LogOn_uname_pwd_00_20.jpg)

## Upload and publish datasets

After completing these steps you will have uploaded and published datasets in SAP Data Intellegence

4.	Click on 'Metadata Explorer'
<br>![](/exercises/ex0/images/DI_HomeScreen_00_30.png)

5.	Click on 'Browse Connections'
<br>![](/exercises/ex0/images/MM_Home_00_40.png)

6.	Click on the 'DI_DATA_LAKE' tile
<br>![](/exercises/ex0/images/BrowseConnection_Select_DI_DATA_LAKE_00_50.png)

7.	Click on the 'shared' tile
<br>![](/exercises/ex0/images/BrowseConnection_Select_shared_00_60.png)

8. Click on the New Folder icon (folder with a +) 
<br>![](/exercises/ex0/images/CreateNewFolder_00_10.png)

9. Enter 'TechEd_DAT163_#' for folder name
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/CreateNewFolder_00_20.png)

10. Click 'OK'
<br>![](/exercises/ex0/images/CreateNewFolder_00_30.png)

11. Click on your newly added 'TechEd_DAT163_#' folder
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/CreateNewFolder_00_40.png)

12. Upload a file, click on the 'Upload Files' icon on the toolbar
<br>![](/exercises/ex0/images/BrowseConnection_UploadFile_00_62.png)

13. Click on the '+' in the upper right hand corner of the Upload Files pop-up window
<br>![](/exercises/ex0/images/BrowseConnection_UploadFilePopUp_00_64.png)

14. Browse to Sample Data folder where you downloaded 'Customer_US.parquet' and 'Sales_data.csv' and select 'Customer_US_#.parquet' 
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/BrowseConnection_UploadCustomerFiles_00_65.png)

15. Click 'Open'
<br>![](/exercises/ex0/images/BrowseConnection_UploadCustomerFiles_00_68.png)

16. Click on the '+' in the upper right hand corner of the Upload Files pop-up window
<br>![](/exercises/ex0/images/BrowseConnection_UploadedCustomer_00_66.png)

17. Select 'Sales_data_#.csv'
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/BrowseConnection_UploadCustomerFiles_00_65_1.png)

18. Click 'Open'
<br>![](/exercises/ex0/images/BrowseConnection_UploadCustomerFiles_00_65_1_Open.png)

19. Click 'Upload'
<br>![](/exercises/ex0/images/BrowseConnection_UploadedSales_00_67.png)

20. After Upload is Complete, click 'Close'
<br>![](/exercises/ex0/images/BrowseConnection_UploadedSales_00_69.png)

21. Click on 'Publication', if not already selected
<br>![](/exercises/ex0/images/BrowseConnection_Name_Desc_00_93.png)

22.	Select 'Customers_US2_#.parquet' file and drag the file to the right and drop in the right pane 'Drag and drop datasets and folders to publish'
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/BrowseConnection_CustomerFiles_00_75.png)

23.	Select 'Sales_data_#.csv' file and drag and drop the file to the right
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/BrowseConnection_DragSales_00_76.png)

24.	Enter 'TechEd_DAT163_#' in the Name parameter and "TechEd_DAT163 Group ## in the Description parameter
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/BrowseConnection_Name_Desc_00_90_Name.png)

25.	Click Publish
<br>![](/exercises/ex0/images/BrowseConnection_Name_Desc_00_90.png)

You have now successfully published two files within SAP Data Intelligence

## Profile and rate the dataset

After completing these steps you will have profiled, viewed the fact sheet, and rate the dataset in SAP Data Intellegence

26. Click the drop down 'Data Intelligence Metadata Explorer' at the top 
<br>![](/exercises/ex0/images/MM_DropDownHome_00_10.png)

27. Click 'Browse Catalog'
<br>![](/exercises/ex0/images/MM_DropDownHome_00_15.png)

28. Click on the 'DI_DATA_LAKE' tile
<br>![](/exercises/ex0/images/BrowseCatalog_DI_DATA_LAKE_00_20.png)

29.	Click on the 'shared' tile
<br>![](/exercises/ex0/images/BrowseCatalog_shared_00_30.png)

30.	Click on the 'TechEd_DAT163_#' tile
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/BrowseCatalog_shared_00_35.png)

31. Hover over Customers_US2_#.parquet and click 'More Action' (three dots) 
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/DataCatalog_SalesProfile_00_40_3dots.png)

32. Select 'Start Profiling'
<br>![](/exercises/ex0/images/DataCatalog_SalesProfile_00_40.png)

33. Click 'Yes' to confirm profiling
<br>![](/exercises/ex0/images/BrowseCatalog_YesProfile_00_50.png)

34. Hover over Sales_data_#.csv file and click 'More Action' (three dots) 
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/DataCatalog_SalesProfile_00_50.png)

35. Select 'Start Profiling'
<br>![](/exercises/ex0/images/DataCatalog_SalesProfile_00_40.png)

36. Click 'Yes' to confirm profiling
<br>![](/exercises/ex0/images/BrowseCatalog_YesProfile_00_55.png)

37. Check 'Notifications' (bell in the upper right hand corner) to verify Customer_US2_#.parquet file has completed profiling
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheetGlasses_00_47.png)

38. Hover over Customers_US2_#.parquet file and click on the 'glasses' to View Fact Sheet
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheetGlasses_00_40.png)

39. View Customer Fact Sheet Overview. Notice you can see the dataset properties, column types, if there are any glossary terms, ratings, comments, discussions and so on associated with this dataset. 
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheetGlasses_00_41.png)

40. Click on Data Preview tab
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheet_00_42_Data.png)

41. Now you can view the actual columns and data within those columns.  Feel free to scroll through the data, notice the country column has 'US', 'USA', 'U.S.A', nulls, and so on.
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheet_00_42_Country.png)

42. Click 'Columns'
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheet_00_140.png)

43. Locate 'Zipcode' to the right of that row click to expand the profiling results for Zipcode, by clicking on '>'
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheet_00_150.png)

44. Scroll to the bottom and locate 'Top 10 Distinct Values'. Notice there an records in the data set that have no Zipcode
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheet_00_160.png)

45. Select the drop down menu for 'Relationships'
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheetViewTree_00_43.png)

46. Select 'Terms and Tags' 
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheetViewTree_00_44.png)

47. Notice there are no glossary terms or tags associated with this dataset
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheetViewTree_00_45.png)

48. Click on 'Reviews' 
<br>![](/exercises/ex0/images/DataCatalog_CustomerFactSheetRatingExisting_00_46.png)

49. Notice this dataset currently has no reviews.  Click on the Stars
<br>![](/exercises/ex0/images/DataCatalog_CustomerReview_00_200.png)

50. Add a 3 star rating by clicking on the 3rd star
<br>![](/exercises/ex0/images/DataCatalog_CustomerReview_00_210.png)

51. Add the following for a Comment: 'US addresses should be standardized to US and this data contains values such as USA, U.S.A. and so on.  Also there are records missing zipcodes, which also does not comply with our standards.'
<br>![](/exercises/ex0/images/DataCatalog_CustomerReview_00_2150.png)

52. Click 'OK'
<br>![](/exercises/ex0/images/DataCatalog_CustomerReview_00_220.png)

You have successfully profiled two datasets, added your ratings and comments based on the profiled results.

## Search, add, and associate a glossary term

After completing these steps you will have search the glossary, added a glossary term, and associated the term with a column in SAP Data Intellegence

53. Click the drop down 'Data Intelligence Metadata Explorer' at the top 
<br>![](/exercises/ex0/images/MM_DropDownHome_00_100.png)

54. Click 'Glossary' on the left hand side
<br>![](/exercises/ex0/images/MM_DropDownHome_00_110.png)

55. Click on 'View Business Glossaries'
<br>![](/exercises/ex0/images/Glossary_MainMenu_00_100.png)

56. Open a the glossary by clicking on the glossary name
<br>![](/exercises/ex0/images/OpenGlossary_00_10.png)

57. There are no terms in this glossary
<br>![](/exercises/ex0/images/Glossary_TermNotFound_00_30.png)

58. Click on the '+' on the right to Create a term
<br>![](/exercises/ex0/images/Glossary_AddTerm_00_40.png)

59. For Name enter 'Address_#'
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/Glossary_Address_00_50.png)

60. For Definition enter 'A collection of information, used to give the location of a building, apartment, or other structure containing street names, house number, city, region, postal code and country.’ 
<br>![](/exercises/ex0/images/Glossary_AddressDefiition_00_60.png)

61. For Keywords type 'street' and press the Enter key
          <br>       type 'city' and press the Enter key
         <br>        type 'state' and press the Enter key
        <br>         type 'zip code' and press the Enter key
        <br> Notice you can have a word or words (phrase) entered for Keywords
<br>![](/exercises/ex0/images/Glossary_AddressKeywords_00_70.png)

62. For Synonyms type 'addr' and press the Enter key 
<br>![](/exercises/ex0/images/Glossary_AddressSaved_00_80.png)

63. Click on 'Save*'
<br>![](/exercises/ex0/images/Glossary_Approve_00_90.png)

64. Click on 'Relationships'
<br>![](/exercises/ex0/images/Glossary_Relationship_00_100.png)

65. Click 'Edit' in the bottom right hand corner
<br>![](/exercises/ex0/images/Glossary_RelationshipsEdit_00_10.png)

66. Click 'Edit Related Objects' 
<br>![](/exercises/ex0/images/Glossary_RelationshipsMain_00_10.png)

67. Click 'Datasets/Columns' 
<br>![](/exercises/ex0/images/Glossary_RelationshipsEditObjects_00_10.png)

68. Expand 'DI_DATA_LAKE' 
<br>![](/exercises/ex0/images/Glossary_RelationshipsExpandTree_00_10.png)

69. Expand 'shared' 
<br>![](/exercises/ex0/images/Glossary_RelationshipsExpandTree_00_11.png)

70. Expand 'TechEd163_#' 
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/Glossary_RelationshipsExpandTree_00_12.png)

71. Select 'Customers_US2.parquet' in the tree structure
<br>![](/exercises/ex0/images/Glossary_RelationshipsExpandTree_00_14_2new10.png)

72. Expand 'Customers_US2.parquet' in the tree structure
<br>![](/exercises/ex0/images/Glossary_RelationshipsExpandTree_00_14.png)

73. Click 'Address1'
<br>![](/exercises/ex0/images/Glossary_RelationshipsColumns_00_10.png)

74. Click on the checkbox for 'Address2
<br>![](/exercises/ex0/images/Glossary_RelationshipsColumns_00_11.png)

75. Click on the checkbox for 'Address3'
<br>![](/exercises/ex0/images/Glossary_RelationshipsColumns_00_12.png)

76. Click on the checkbox for 'City'
<br>![](/exercises/ex0/images/Glossary_RelationshipsColumns_00_12_2new.png)

77. Click on the checkbox for 'State'
<br>![](/exercises/ex0/images/Glossary_RelationshipsColumns_00_12_2new_10.png)

78. Click on the checkbox for 'Zipcode'
<br>![](/exercises/ex0/images/Glossary_RelationshipsColumns_00_12_2new_20.png)

79.  Click 'Save Related Objects' located in the bottom right hand corner. 
<br>![](/exercises/ex0/images/Glossary_RelationshipsSavedAssociationLineage_00_10.png)

80. You have created a relationship with the Address glossary term and columns that create an address in your customer parquet file
<br>![](/exercises/ex0/images/Glossary_RelationshipsSavedAssociationLineage_00_12.png)

81. Click the drop down 'Data Intelligence Metadata Explorer' at the top 
<br>![](/exercises/ex0/images/MM_DropDownHome_00_12.png)

82. Click 'Catalog'
<br>![](/exercises/ex0/images/MM_DropDownHome_00_14.png)

83. Click 'Browse Catalog'
<br>![](/exercises/ex0/images/MM_DropDownHome_00_16.png)

84. Click on the 'DI_DATA_LAKE' tile
<br>![](/exercises/ex0/images/BrowseCatalog_DI_DATA_LAKE_00_120.png)

85.	Click on the 'shared' tile
<br>![](/exercises/ex0/images/BrowseCatalog_shared_00_130.png)

86. Expand 'TechEd163_#' 
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/BrowseCatalog_shared_00_140.png)

87. Select on Customers_US2_#.parquet file and on the right side scroll down to Glossary and see the associated term 'Add 
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex0/images/Glossary_Catalog_Relationships_00_10.png)

You have added a glossary term of 'Address' with a definition, synonym, and keywords.  You have also created a relationship between the glossary term 'Address' and with the Customer_US dataset, as well as, columns within that dataset that make up and address.
 
 ## Summary

Now that you have completed the data catalog by uploading datasets, profiling datasets, rating and commenting on datasets, and using the glossary, lets continue by creating and using validation and quality rules against the data. 
Continue to - [Exercise 2 - Rule Creation, Testing Rule, Rulebooks, and Data Quality Dashboards](../ex1/README.md)
