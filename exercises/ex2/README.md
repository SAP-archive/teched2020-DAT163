# Exercise 2 - Exercise 2 Description

In this exercise, we will use self-service data prepartion to correct the country, run the country US rule after using data preparation and review the results, and we will view the data lineage.

## Exercise 2.1 Sub Exercise 1 Description

After completing these steps you will have corrected the data through self-service data preparation.

1. Click on the 'Data Intelligence Metadata Explorer' drop down 
<br>![](/exercises/ex2/images/DataPrep_DI_MM_Home_02_10_1new.png)

2. Click on 'Catalog'
<br>![](/exercises/ex2/images/DataPrep_DI_MM_BrowseCat_02_10_add.png)

2.	Select 'Browse the Catalog'
<br>![](/exercises/ex2/images/DataPrep_DI_MM_BrowseCat_02_10_1new1.png)

3. Enter '##' in the Search entire catalog text box
<br>Note: replace ## with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_DI_SearchCat_02_10.png)

4. Hover over your 'Customers_US2.parquet##' file and click on the glasses icon to view the factsheet
<br>Note: replace ## with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_CustomersFactsheet_02_10.png)

5. Click on 'Columns' 
<br>![](/exercises/ex2/images/DataPrep_FactSheet_DistinctValue_02_10.png)

5. Click on the 'Country' column name 
<br>![](/exercises/ex2/images/DataPrep_FactSheet_DistinctValue_02_110.png)

7. Scroll down to see the 'Data Preview' and the 'Top 10 Disctint Values' panes.  Notice the distinct values in this column are 'US', 'U.S.A.', 'USA', 'U.S.', and nulls.  This dataset is for US and the country column should have the same value for all the records.
<br>![](/exercises/ex2/images/DataPrep_FactSheet_DistinctValue_02_120.png)

6. Click on the 'Reviews' 
<br>![](/exercises/ex2/images/DataPrep_Comments_02_10.png)

7. Notice the comment states the records should all follow the standards of 'US' for this US customer file. 
<br>![](/exercises/ex2/images/DataPrep_Comments_02_110.png)

8. Click on 'Prepare Data' icon located on the right hand side
<br>![](/exercises/ex2/images/DataPrep_StartPrep_02_10.png)

9. Click the 'Country' column
<br>![](/exercises/ex2/images/DataPrep_SelectCountryCol_02_10.png)

10. Click on 'Replace' under Actions on the right
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_10.png)

11. Your organization's standard is for the United States country values to be 'US'.  For Replace leave the Search on 'Custom String'.  Notice the second row has a country of 'USA'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_20.png)

12. For the value enter 'USA'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_120.png)

13. For the Replace by, enter 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_130.png)

14. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_30.png)

15. Notice the second row's 'Country' value of 'USA' have been replaced with 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_140_1new.png)

16. Click on 'Replace'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_10.png)

17. For the value enter 'U.S.A'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_150.png)

18. For the Replace by, enter 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_160.png)

19. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_170.png)

20. Click on 'Replace'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_10.png)

21. For the value enter 'U.S.'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_150_new.png)

22. For the Replace by, enter 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_160_new.png)

23. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_170_new.png)

24. Click on 'Replace'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_10.png)

25. Click on the dropdown for search and change 'Custom String' to 'NULL'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_180_new.png)

26. For Replace by, leave 'Custom String' and add the value 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_190_new.png)

27. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_195_new.png)

28. Notice the values under the 'Country' column have all been replaced with 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_197_new.png)

29. Your organizational standard is also to have one address line and this dataset has three, so we will combine them so we have one address column, without losing any data.
<br>Click on the 'Address1' header column
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_10.png)

30. Click 'Combine' on the right hand side
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_20.png)

31. Click on 'Address2'
<br> Note: Depending on screen size you may need to scroll down under 'Combine with:'
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_30.png)

32. Click on 'Address3'
<br> Note: Depending on screen size you may need to scroll down under 'Combine with:'
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_40.png)

33. For 'Combine using:' enter a ' ' (click the spacebar) for the Separator
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_50.png)

34. For New Column Name* enter 'Full_Address'
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_60.png)

35. Click Apply
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_70.png)

36. After 'Address3' column you will now see your new 'Full_Address' column that now contains the complete address
<br> Note: Depending on screen size you may need to scroll to the right to see 'Full_Address'
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_80.png)

37. Click on the 'Data Intelligence Metadata Explorer' drop down
<br>![](/exercises/ex2/images/DataPrep_DI_DropDown_02_10.png)

38. Select 'Browse Catalog'
<br>![](/exercises/ex2/images/DataPrep_DI_DropDowBrowse_Catalog_02_10.png)

39. Enter 'sales*' in the Search entire catalog text box
<br>![](/exercises/ex2/images/DataPrep_SearchCatalog_02_10.png)

40. Hover over 'Sales_data_##.csv' and click on the '...'
<br>Note: replace ## with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_SalesData_02_05.png)

41. Choose 'Prepare Data'
<br>![](/exercises/ex2/images/DataPrep_SalesData_02_10.png)

42. Notice the sales data has 'TRANS_ID', 'CUST_ID', 'TRANS_AMT', and 'TRANS_DATE', but you cannot see the customer details, such as name, address, and so on.  Click on the 'Actions' on the right hand side.
<br>![](/exercises/ex2/images/DataPrep_SalesData_02_120_new.png)

43. Click on 'Actions' on the right, if not already selected
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_15_new.png)

44. Select 'Enrich Preparation'
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_10.png)

45. You want to do a Left Outer Join, which will includes all rows from the both datasets.  Select 'Customers_US2_##' on the left hand side under 'Preparations'
<br>Note: replace ## with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_30.png)

46. Drag 'Customers_US2_##' to the 'Drop here to merge' that is to the left of the 'S1' in the center
<br>Note: replace ## with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_40.png)

47. Select 'Left Join
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_50.png)

48. Change 'TRANS_ID' to 'CUST_ID'.  This will allow you to join the two datasets on the common column of customer id.
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_60.png)

49. Uncheck 'Address1', 'Address2', and 'Address2'.  We don't want to add these fields because we now have the address data in one column called 'Full_Address'
<br> Note: This will allow you to join the two datasets on the common column of customer id.
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_160_new.png)

50. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_70.png)

51. Notice the data no longer contains 'Address1', 'Address2', or 'Address3', but does contain 'Full_Address'
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_180_new.png)

52. Scroll to the right and notice the customer data now has 'TRANS_ID', 'CUST_ID', 'TRANS_AMT', and 'TRANS_DATE' data associated to it.
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_80.png)

53. Click 'Apply Enrichment' at the bottom right hand corner
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_90.png)

54. Click on 'Actions'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new15.png)

******************************
54. Notice there are duplicate ID/CUST_ID and we need a total of all transactions per customer id
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new180.png)

54. Click on 'Actions'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new15.png)

55. Click on 'Aggregate Preparation'
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new10.png)

56. Select all columns - click on the first column hold the Shift key and scroll to the last column in the list and select, so all columns are highlighted
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new20.png)

57. Drag and drop all columns in the Output Columns pane
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new30.png)

58. Click on the drop down for Zipcode
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new40.png)

59. Change to 'No Aggregation'
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new50.png)

60. Click on the drop down for CUST_ID
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new60.png)

59. Change to 'No Aggregation'
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new70.png)

60. Click on the 'X' fpr 'TRANS_DATE' to delete the column
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new80.png)

61. Click on the 'X' fpr 'Date' to delete the column
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new90.png)

62. Click on the 'X' fpr 'TRANS_ID' to delete the column
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new100.png)

63. Click on the 'X' fpr 'ID' to delete the column
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new110.png)

64. Click on 'CUST_ID' column
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new120.png)

65. Drag and drop the 'CUST_ID' column so it is first in the list of Output Columns
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new130.png)

66. Click on 'TRANS_AMT' column
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new140.png)

67. Drag and drop the 'TRANS_AMT' column so after 'CUST_ID' in the list of Output Columns
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new150.png)

68. All rows with the same CUST_ID now have a total for TRANS_AMT, instead of each transaction listed separately
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new160.png)

69. Click 'Apply Aggregation'
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new170.png)














******************************

55. Click on 'Run Preparation'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new20.png)

56. Click on the browse icon for the 'Container:' parameter
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new30.png)

57. Click on 'TechEd_DAT163_##'
<br>Note: replace ## with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new40.png)

58. Enter Customer_Sales_##' for Dataset Name
<br>Note: replace ## with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new70.png)

60. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new80.png)

65. Click on 'Manage Preparation Tasks
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_140_1new_20.png)

66. Check to make sure you prepartions are successfull.  You can click on the 'Refresh' icon, to see that the preparation has completed.
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_140_1new_30.png)



<br><br><br><br>
<br>
<br>
<br>
<br>
<br>
<br><br><br><br>



62. Click on the ellipsis (...) for 'Customer_Sales_##.csv'
<br>Note: replace ## with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_50.png)

63. Click on 'View Fact Sheet' to view the data
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_60.png)

64. Click on 'Data Preview' to view the data
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_65.png)

65. Notice the data contains only 1 address column and also contains all the sales transactional data in one file.
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_70_new.png)



<br><br><br><br>
<br>
<br>
<br>
<br>
<br>
<br><br><br>

Bind our new 'Customer_Sales_##' to our country rule

85. Click on 'Data Intelligence Metadata Explorer'
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_10_1new10.png)

86. Click on 'View Rulebooks' from withing Rules
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_10.png)

87. Click on your 'TechEdDAT163_##'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_30.png)

88. Expand Accuracy rule category by clicking on the '>'
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_1new_10.png)

89. Click on the ellipsis (...) to the right under Rule Bindings
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_20.png)

90. Click on 'View Rule Bindings'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_30.png)

91. Click on the upper '+' in the upper right hand corner to Create a Rule Binding
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_40.png)

92. Click on the 'Browse' icon for 'Qualified Name'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_50.png)

93. Click on 'Browse'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_60.png)

94. Click on the drop down arrow for 'Connections'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_70.png)

94. Select 'DI_DATA_LAKE'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_80.png)

95. Select on 'shared'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_90.png)

96. Select 'TechEd_DAT163_##'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_95.png)

97. Select 'Customer_Sales_##'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_100.png)

98. Click 'OK'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_110.png)

99. Click 'Save'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_120.png)

100. Click 'Run All'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_130.png)

101. Click on 'Data Intelligence Metadata Explorer'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new10.png)

102. Click on 'Monitor'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new20.png)

103. Click on 'Monitor Tasks'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new30.png)

104. Notice your Rulebook is running
<br>![](/exercises/ex2/images/DataPrep_Monitor_02_10_1new10.png)

105. Wait for you Rulebook to Complete
<br>![](/exercises/ex2/images/DataPrep_Monitor_02_10_1new20.png)

106. Click on 'Data Intelligence Metadata Explorer'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new10.png)

107. Click on 'Rules'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new40.png)

108. Click on 'View Rulebooks'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new50.png)

109. Click on your 'TechEdDAT163_##'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_30.png)

110. Click on 'View Results'
<br>![](/exercises/ex2/images/DataPrep_RuleBookResults_02_1new10.png)

111. Notice your quality has improved from your Data Preparation
<br>![](/exercises/ex2/images/DataPrep_RuleBookResults_02_1new20.png)

112. Click on 'View Rules Dashboards'
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_10_1new10.png)

113.  'TechEd_DAT163_##'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_20.png)

114. Click on the pencil icon located on the right hand side
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_30.png)

115. Click on the '+' (plus sign) located next to your first dashboard
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_40.png)

116. Click on the drop down and select 'TechEd_DAT163_##'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_50.png)

117. Click on 'Step 2'
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_60.png)

117. Click on 'Step 3'
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_70.png)

118. Select 'Single Dataset'
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_80.png)

119. Click on 'Step 4'
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_90.png)

120. Click on 'Select Customer_Sales_##'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_100.png)

121. Click on 'Step 5'
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_110.png)

122. Click on 'Save'
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_120.png)

123. You have now created a new dashboard for your combined Customer and Sales file
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_130.png)






************************




124. Click on 'Data Intelligence Metadata Explorer'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new10.png)

125. Select 'Home'
<br>![](/exercises/ex2/images/DataPrep_DIMenuHome_02_10_1new10.png)

126. Click 'View Preparations'
<br>![](/exercises/ex2/images/DataPrep_ViewPreo_02_10_1new10.png)

127. Click on 'Customer_Sales_##'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new20.png)

127. Select 'Actions'
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new30.png)

127. Select 'Manage Preparation Tasks'
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new40.png)

128. Click on the ellipsis (...) for 'Customer_Sales_##.csv'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new50.png)

129. Select 'View Fact Sheet'
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new60.png)

130. Start Profiling by clicking in the Run icon on the right hand side
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new70.png)

130. Click 'Yes' to confirm profiling
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new80.png)

131. Wait for profiling to complete by checking the notification icon (bell) located in the upper right hand corner
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new90.png)








<br><br><br><br>
<br>
<br>
<br>
<br>
<br>
<br><br><br>

66. Click on 'Recipe'
<br>![](/exercises/ex2/images/DataPrep_LimitColumns_02_10.png)

67. Click on the pencil to edit
<br>![](/exercises/ex2/images/DataPrep_LimitColumns_02_10.png)

68. Click on the join icon between the customer and sales datasets
<br>![](/exercises/ex2/images/DataPrep_LimitColumns_02_20.png)

69. Uncheck 'Address1', 'Address2', and 'Address3', since we have now combined those 3 columns into one column called, 'Full_Address'
<br>![](/exercises/ex2/images/DataPrep_LimitColumns_02_30.png)

70. CLick 'Apply'
<br>![](/exercises/ex2/images/DataPrep_LimitColumns_02_30.png)

71. Select 'Run Preparation'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_20.png)

72. Click on the browse icon for the Container parameter
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_30.png)

73. Browse to 'TechEdDAT163_##' folder
<br>Note: replace ## with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_30.png)

74. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_40.png)

75. For Dataset Name: enter ' Customer_Sales_##'
<br>Note: replace ## with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_35.png)

76. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_35.png)

77. Click 'Yes' on the Warning pop up letting you know the schema doesn't' match (remember we remove Address1 to Address3 columns), so you want to overwrite the schema with the new updatd schema
<br>![](/exercises/ex2/images/DataPrep_LimitColumns_02_40.png)

78. Click Action
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10.png)

79. Select 'Manage Preparation Tasks'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_20.png)

80. We can view the status
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_50.png)

81. Click the Refresh icon to check when tasks are completed
<br>![](/exercises/ex2/images/DataPrep_RefreshStatus_02_10.png)
 
82. Click on the glasses icon when the status shows complete
<br>![](/exercises/ex2/images/DataPrep_RefreshGlasses_02_10.png)

83. Click 'Data Preview'
<br>![](/exercises/ex2/images/DataPrep_RefreshDataPreview_02_10.png)

84. Notice there is only 'Full_Address' now, Address1, Address2, and Address3 have been removed
<br>![](/exercises/ex2/images/DataPrep_RefreshDataPreview_02_10.png)

# Add Aggregated of sales data

85. Click on 'Data Intelligence Metadata Explorer'
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_10.png)

86. Click on 'View Rulebooks'
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_10.png

87. In the 'Filter rulebooks names' enter 'Tech"
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_20.png)

88. Click on your 'TechEdDAT163_##'
<br>Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_30.png)

89. 


where ## is the group number assigned to you







## Summary

You've now ...

Continue to - [Exercise 3 - Excercise 3 ](../ex3/README.md)
