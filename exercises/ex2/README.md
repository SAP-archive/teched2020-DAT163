# Exercise 2 - Exercise 2 Description

In this exercise, we will use self-service data prepartion to correct the country, run the country US rule after using data preparation and review the results, and we will view the data lineage.

## Exercise 2.1 Sub Exercise 1 Description

After completing these steps you will have corrected the data through self-service data preparation.

1. Click on the 'Data Intelligence Metadata Explorer' drop down 
<br>![](/exercises/ex2/images/DataPrep_DI_MM_Home_02_10.png)

2.	Select 'Browse the Catalog'
<br>![](/exercises/ex2/images/DataPrep_DI_MM_BrowseCat_02_10.png)

3. Enter '##' in the Search entire catalog text box
where ## is the group number assigned to you
<br>![](/exercises/ex2/images/DataPrep_DI_SearchCat_02_10.png)

4. Hover over your 'Customers_US2.parquet##' file and click on the glasses icon to view the factsheet
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_CustomersFactsheet_02_10.png)

5. Click on 'Column' 
<br>![](/exercises/ex2/images/DataPrep_FactSheet_DistinctValue_02_10.png)

5. Click on the 'Country' column name 
<br>![](/exercises/ex2/images/DataPrep_FactSheet_DistinctValue_02_110.png)

6. Scroll down to see the 'Data Preview' and the 'Top 10 Disctint Values' panes.  Notice the distinct values in this column are 'US', 'U.S.A.', 'USA', 'U.S.', and nulls.  This dataset is for US and the country column should have the same value for all the records.
<br>![](/exercises/ex2/images/DataPrep_FactSheet_DistinctValue_02_120.png)

6. Click on the 'Reviews' 
<br>![](/exercises/ex2/images/DataPrep_Comments_02_10.png)

7. Notice the comment states the records should all follow the standards of 'US' for this US customer file. 
<br>![](/exercises/ex2/images/DataPrep_Comments_02_110.png)

8. Click on'Prepare Data' icon located on the right hand side
<br>![](/exercises/ex2/images/DataPrep_StartPrep_02_10.png)

9. Click the 'Country' column
<br>![](/exercises/ex2/images/DataPrep_SelectCountryCol_02_10.png)

10. Click on 'Replace'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_10.png)

11. Your organization's standard is for the United States country values to be 'US'.  For Replace leave the Search on 'Custom String'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_20.png)

12. For the value enter 'USA'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_120.png)

13. For the Replace by, enter 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_130.png)

13. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_30.png)

13. Notice the values under the 'Country' column that were 'USA' have been replaced with 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_140.png)

10. Click on 'Replace'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_10.png)

12. For the value enter 'U.S.A'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_150.png)

13. For the Replace by, enter 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_160.png)

13. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_170.png)

10. Click on 'Replace'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_10.png)

12. For the value enter 'U.S.'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_150.png)

13. For the Replace by, enter 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_160.png)

13. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_170.png)

10. Click on 'Replace'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_10.png)

11. Click on the dropdown for search and change 'Custom String' to 'NULL'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_180.png)

11. For Replace by, leave 'Custom String' and add the value 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_190.png)

13. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_195.png)

13. Notice the values under the 'Country' column have all been replaced with 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_197.png)

27. Your organizational standard is also to have one address line and this dataset has three, so we will combine them so we have one address column, without losing any data.
Click on the 'Address1' column
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_10.png)

28. Click 'Combine' on the right hand side
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_20.png)

29. Click on 'Address2'
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_30.png)

30. Click on 'Address3'
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_40.png)

31. For Combine using: enter a ' ' (space) for the Separator
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_50.png)

32. For New Column Name* enter 'Full_Address'
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_60.png)

33. Click Apply
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_70.png)

34. After 'Address3' column you will now see your new 'Full_Address' column that now contains the complete address
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_80.png)

35. Click on the 'Data Intelligence Metadata Explorer' drop down
<br>![](/exercises/ex2/images/DataPrep_DI_DropDown_02_10.png)

36. Select 'Browse Catalog'
<br>![](/exercises/ex2/images/DataPrep_DI_DropDowBrowse_Catalog_02_10.png)

37. Enter 'sales*' in the Search entire catalog text box
<br>![](/exercises/ex2/images/DataPrep_SearchCatalog_02_10.png)

38. Hover over 'Sales_data_##.csv' and click on the '...'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_SalesData_02_05.png)

39. Choose 'Prepare Data'
<br>![](/exercises/ex2/images/DataPrep_SalesData_02_10.png)

40. Notice the sales data has 'TRANS_ID', 'CUST_ID', 'TRANS_AMT', and 'TRANS_DATE', but you cannot see the customer details, such as name, address, and so on.  Click on the 'Actions' on the right hand side.
<br>![](/exercises/ex2/images/DataPrep_SalesData_02_120.png)

41. Select 'Enrich Preparation'
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_10.png)

37. You want to do a Left Outer Join, which will includes all rows from the both datasets, where an inner join would only include matching rows from the datasets.  Select 'Customers_US2_##'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_30.png)

38. Drag 'Customers_US2_##' to the 'Drop here to merge' that is to the left of the 'S1' in the center
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_40.png)

39. Select 'Left Join
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_50.png)

40. Change 'TRANS_ID' to 'CUST_ID'.  This will allow you to join the two datasets on the common column of customer id.
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_60.png)

40. Uncheck 'Address1', 'Address2', and 'Address2'.  We don't want to add these fields because we now have the address data in one column called 'Full_Address'
<br> Note: This will allow you to join the two datasets on the common column of customer id.
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_160.png)

41. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_70.png)

42. Notice the data no longer contains 'Address1', 'Address2', or 'Address3', but does contain 'Full_Address'
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_180.png)

42. Scroll to the right and notice the customer data now has 'TRANS_ID', 'CUST_ID', 'TRANS_AMT', and 'TRANS_DATE' data associated to it.
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_80.png)

43. Click 'Apply Enrichment' at the bottom right hand corner
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_90.png)

44. Click Action
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10.png)

45. Select 'Run Preparation'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_20.png)

46. Click on the browse icon for the Container parameter
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_30.png)

47. Select to 'TechEd_DAT163_##' folder
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_30.png)

47. Select to 'Customers_US2_##.parquet' file
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_35.png)

47. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_140.png)

48. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_135.png)

1. Click on the 'Data Intelligence Metadata Explorer' drop down 
<br>![](/exercises/ex2/images/DataPrep_DI_MM_Home_02_110.png)

2.	Select 'Monitor'
<br>![](/exercises/ex2/images/DataPrep_DI_MM_BrowseCat_02_120.png)

2.	Select 'Monitor Tasks'
<br>![](/exercises/ex2/images/DataPrep_DI_MM_BrowseCat_02_130.png)

2.	Check to see when you Preparation task changes from 'Pending' to 'Completed'
<br>![](/exercises/ex2/images/DataPrep_DI_MM_BrowseCat_02_140.png)

1. When the Preparation task is complete, click on the 'Data Intelligence Metadata Explorer' drop down 
<br>![](/exercises/ex2/images/DataPrep_DI_MM_Home_02_110.png)

2.	Select 'Catalog'
<br>![](/exercises/ex2/images/DataPrep_DI_MM_BrowseCat_02_110.png)

2.	Select 'Browse the Catalog'
<br>![](/exercises/ex2/images/DataPrep_DI_MM_BrowseCat_02_10.png)

3. Select 'DI_DATA_LAKE'
<br>![](/exercises/ex2/images/DataPrep_DIDATALAKE_02_10.png)

3. Select 'shared'
<br>![](/exercises/ex2/images/DataPrep_DIDATALAKE_02_20.png)

4. Select 'TechEd_DAT163_##' 
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_DIDATALAKE_02_30.png)

4. Hover over 'Customers_US2_##.parquet' and click on the glass to 'View Fact Sheet'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_Mng_Prep_02_10.png)

8. Click on'Prepare Data' icon located on the right hand side
<br>![](/exercises/ex2/images/DataPrep_StartPrep_02_10.png)

9. Click on the existing preparation
<br>![](/exercises/ex2/images/DataPrep_Mng_Prep_02_20.png)

49. Click Action
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10.png)

50. Select 'Manage Preparation Tasks'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_20.png)







51. We can view the status
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_50.png)

69. Click the Refresh icon to check when tasks are completed
<br>![](/exercises/ex2/images/DataPrep_RefreshStatus_02_10.png)

52. Click on the glasses icon
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_50.png)

53. Click on 'Data Preview' to view the data
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_60.png)

54. Click on 'Recipe'
<br>![](/exercises/ex2/images/DataPrep_LimitColumns_02_10.png)

55. Click on the pencil to edit
<br>![](/exercises/ex2/images/DataPrep_LimitColumns_02_10.png)

56. Click on the join icon between the customer and sales datasets
<br>![](/exercises/ex2/images/DataPrep_LimitColumns_02_20.png)

57. Uncheck 'Address1', 'Address2', and 'Address3', since we have now combined those 3 columns into one column called, 'Full_Address'
<br>![](/exercises/ex2/images/DataPrep_LimitColumns_02_30.png)

58. CLick 'Apply'
<br>![](/exercises/ex2/images/DataPrep_LimitColumns_02_30.png)

59. Select 'Run Preparation'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_20.png)

60. Click on the browse icon for the Container parameter
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_30.png)

61. Browse to 'TechEdDAT163_##' folder
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_30.png)

63. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_40.png)

64. For Dataset Name: enter ' Customer_Sales_##'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_35.png)

65. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_35.png)

66. Click 'Yes' on the Warning pop up letting you know the schema doesn't' match (remember we remove Address1 to Address3 columns), so you want to overwrite the schema with the new updatd schema
<br>![](/exercises/ex2/images/DataPrep_LimitColumns_02_40.png)

67. Click Action
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10.png)

67. Select 'Manage Preparation Tasks'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_20.png)

68. We can view the status
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_50.png)

69. Click the Refresh icon to check when tasks are completed
<br>![](/exercises/ex2/images/DataPrep_RefreshStatus_02_10.png)
 
70. Click on the glasses icon when the status shows complete
<br>![](/exercises/ex2/images/DataPrep_RefreshGlasses_02_10.png)

71. Click 'Data Preview'
<br>![](/exercises/ex2/images/DataPrep_RefreshDataPreview_02_10.png)

72. Notice there is only 'Full_Address' now, Address1, Address2, and Address3 have been removed
<br>![](/exercises/ex2/images/DataPrep_RefreshDataPreview_02_10.png)

# Add Aggregated of sales data

73. Click on 'Data Intelligence Metadata Explorer'
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_10.png)

74. Click on 'View Rulebooks'
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_10.png

75. In the 'Filter rulebooks names' enter 'Tech"
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_20.png)

76. Click on your 'TechEdDAT163_##'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_30.png)

78. 


where ## is the group number assigned to you







## Summary

You've now ...

Continue to - [Exercise 3 - Excercise 3 ](../ex3/README.md)
