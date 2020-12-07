# Objective

As a Business Analyst you want to discover the data, gain insight into the data, and enhance and enrich the data through self-service data preparation.  In this exercise, we will use self-service data prepartion to correct the country, run the country US rule after using data preparation, and review the results, and we will view the data lineage.

## Self-Service Data Preparation

After completing these steps you will have corrected the data through self-service data preparation.

1. Click on the 'Data Intelligence Metadata Explorer' drop down 
<br>![](/exercises/ex2/images/DataPrep_DI_MM_Home_02_10_1new.png)

2. Click on 'Catalog'
<br>![](/exercises/ex2/images/DataPrep_DI_MM_BrowseCat_02_10_add.png)

3.	Select 'Browse the Catalog'
<br>![](/exercises/ex2/images/DataPrep_DI_MM_BrowseCat_02_10_1new1.png)

4. Enter '#' in the Search entire catalog text box
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_DI_SearchCat_02_10.png)

5. Hover over your 'Customers_US2.parquet_#' file and click on the glasses icon to view the Fact Sheet
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_CustomersFactsheet_02_10.png)

6. Click on 'Columns' 
<br>![](/exercises/ex2/images/DataPrep_FactSheet_DistinctValue_02_10.png)

7. Click on the 'Country' column name 
<br>![](/exercises/ex2/images/DataPrep_FactSheet_DistinctValue_02_110.png)

8. Scroll down to see the 'Data Preview' and the 'Top 10 Disctint Values' panes.  Notice the distinct values in this column are 'US', 'U.S.A.', 'USA', 'U.S.', and nulls.  This dataset is for US and the country column should have the same value for all the records.
<br>![](/exercises/ex2/images/DataPrep_FactSheet_DistinctValue_02_120.png)

9. Click on the 'Reviews' 
<br>![](/exercises/ex2/images/DataPrep_Comments_02_10.png)

10. Notice the comment states the records should all follow the standards of 'US' for this US customer file. 
<br>![](/exercises/ex2/images/DataPrep_Comments_02_110.png)

11. Click on 'Prepare Data' icon located on the right hand side
<br>![](/exercises/ex2/images/DataPrep_StartPrep_02_10.png)

12. Click the 'Country' column (select the Country column)
<br>![](/exercises/ex2/images/DataPrep_SelectCountryCol_02_10.png)

13. Click on 'Replace' under Actions on the right
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_10.png)

14. Your organization's standard is for the United States country values to be 'US'.  For Replace leave the Search on 'Custom String'.  Notice the second row in the data preview has a country of 'USA'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_20.png)

15. For the Search value enter 'USA'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_120.png)

16. For the Replace by, enter 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_130.png)

17. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_30.png)

18. Notice the second row's 'Country' value of 'USA' have been replaced with 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_140_1new.png)

19. Click on 'Replace'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_10.png)

20. For the value enter 'U.S.A'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_150.png)

21. For the Replace by, enter 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_160.png)

22. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_170.png)

23. Click on 'Replace'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_10.png)

24. For the value enter 'U.S.'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_150_new.png)

25. For the Replace by, enter 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_160_new.png)

26. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_170_new.png)

27. Click on 'Replace'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_10.png)

28. Click on the dropdown for search and change 'Custom String' to 'NULL'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_180_new.png)

29. For Replace by, leave 'Custom String' and add the value 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_190_new.png)

30. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_195_new.png)

31. Notice the values under the 'Country' column have all been replaced with 'US'
<br>![](/exercises/ex2/images/DataPrep_SelectCountryReplace_02_197_new.png)

32. Your organizational standard is also to have one address line and this dataset has three, so we will combine them so we have one address column, without losing any data.
<br>Click on the 'Address1' header column
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_10.png)

33. Click 'Combine' on the right hand side
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_20.png)

34. Click on 'Address2'
<br> Note: Depending on screen size you may need to scroll down under 'Combine with:'
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_30.png)

35. Click on 'Address3'
<br> Note: Depending on screen size you may need to scroll down under 'Combine with:'
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_40.png)

36. For 'Combine using:' enter a ' ' (click the spacebar) for the Separator
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_50.png)

37. For New Column Name* enter 'Full_Address'
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_60.png)

38. Click Apply
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_70.png)

39. After 'Address3' column you will now see your new 'Full_Address' column that now contains the complete address
<br> Note: Depending on screen size you may need to scroll to the right to see 'Full_Address'
<br>![](/exercises/ex2/images/DataPrep_AddressPrep_02_80.png)

40. Click on the 'Data Intelligence Metadata Explorer' drop down
<br>![](/exercises/ex2/images/DataPrep_DI_DropDown_02_10.png)

41. Select 'Browse Catalog'
<br>![](/exercises/ex2/images/DataPrep_DI_DropDowBrowse_Catalog_02_10.png)

42. Enter '#' in the Search entire catalog text box
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_SearchCatalog_02_10.png)

43. Hover over 'Sales_data_#.csv' and click on the '...'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_SalesData_02_05.png)

44. Choose 'Prepare Data'
<br>![](/exercises/ex2/images/DataPrep_SalesData_02_10.png)

45. Notice the sales data has 'TRANS_ID', 'CUST_ID', 'TRANS_AMT', and 'TRANS_DATE', but you cannot see the customer details, such as name, address, and so on.  Click on the 'Actions' on the right hand side.
<br>![](/exercises/ex2/images/DataPrep_SalesData_02_120_new.png)

46. Click on 'Actions' on the right, if not already selected
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_15_new.png)

47. Select 'Enrich Preparation'
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_10.png)

48. You want to do a Left Outer Join, with your customer file, this will includes all rows from the both datasets.  Select 'Customers_US2_#' on the left hand side under 'Preparations'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_30.png)

49. Drag 'Customers_US2_#' to the 'Drop here to merge' that is to the left of the 'S1' in the center
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_40.png)

50. Select 'Left Join
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_50.png)

51. Click on the ID column heading
<br>![](/exercises/ex2/images/DataPrep_Sort_02_2new10.png)

51. Click on the three horizontal lines, to open column menu
<br>![](/exercises/ex2/images/DataPrep_Sort_02_2new20.png)

51. Change 'TRANS_ID' to 'CUST_ID'.  This will allow you to join the two datasets on the common column of customer id.
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_60.png)

52. Uncheck 'Address1', 'Address2', and 'Address2'.  We don't want to add these fields because we now have the address data in one column called 'Full_Address'
<br> Note: This will allow you to join the two datasets on the common column of customer id.
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_160_new.png)

53. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_70.png)

54. Notice the data no longer contains 'Address1', 'Address2', or 'Address3', but does contain 'Full_Address'
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_180_new.png)

55. Scroll to the right and notice the customer data now has 'TRANS_ID', 'CUST_ID', 'TRANS_AMT', and 'TRANS_DATE' data associated to it.
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_80.png)

56. Click 'Apply Enrichment' at the bottom right hand corner
<br>![](/exercises/ex2/images/DataPrep_ActionJoin_02_90.png)

57. Click on 'Actions'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new15.png)

58. There are duplicate ID/CUST_ID and we need a total of all transactions per customer id
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new180.png)

59. Click on 'Actions'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new15.png)

60. Click on 'Aggregate Preparation'
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new10.png)

61. Select all columns - click on the first column hold the Shift key and scroll to the last column in the list and select, so all columns are highlighted
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new20.png)

62. Drag and drop all columns in the Output Columns pane
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new30.png)

63. Click on the drop down for Zipcode
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new40.png)

64. Change to 'No Aggregation'
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new50.png)

65. Click on the drop down for CUST_ID
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new60.png)

66. Change to 'No Aggregation'
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new70.png)

67. Click on the 'X' fpr 'TRANS_DATE' to delete the column
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new80.png)

68. Click on the 'X' fpr 'Date' to delete the column
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new90.png)

69. Click on the 'X' fpr 'TRANS_ID' to delete the column
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new100.png)

70. Click on the 'X' fpr 'ID' to delete the column
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new110.png)

71. Click on 'CUST_ID' column
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new120.png)

72. Drag and drop the 'CUST_ID' column so it is first in the list of Output Columns
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new130.png)

73. Click on 'TRANS_AMT' column
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new140.png)

74. Drag and drop the 'TRANS_AMT' column so after 'CUST_ID' in the list of Output Columns
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new150.png)

75. All rows with the same CUST_ID now have a total for TRANS_AMT, instead of each transaction listed separately
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new160.png)

76. Click 'Apply Aggregation'
<br>![](/exercises/ex2/images/DataPrep_Aggregate_02_10_1new170.png)

77. Click on 'Actions'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new15.png)

77. Click on 'Run Preparation'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new20.png)

78. Click on the browse icon for the 'Container:' parameter
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new30.png)

79. If your container already has your '/shared/TechEd_DAT163_#' listed skip, if not select your 'TechEd_DAT163_#' and click 'Apply'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new40.png)

80. Enter Customer_Sales_#' for Dataset Name
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new70.png)

81. Click 'Apply'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new80.png)

82. Click on 'Actions'
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_10_1new15.png)

83. Click on 'Manage Preparation Tasks
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_140_1new_20.png)

84. Check to make sure you prepartions are successfull.  You can click on the 'Refresh' icon, to see that the preparation has completed.
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_140_1new_30.png)

85. Click on the ellipsis (...) for 'Customer_Sales_#.csv'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_50.png)

86. Click on 'View Fact Sheet' to view the data
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_60.png)

87. Click on 'Data Preview' to view the data
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_65.png)

88. Notice the data contains only 1 address column; the CUST_ID with no duplicate customer ids; and a TRANS_AMT column showing the total sold to a given customer in one file.
<br>![](/exercises/ex2/images/DataPrep_ActionSave_02_70_new.png)

89. To profile this new data set click on the Run icon on the right hand side
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new70.png)

90. Click 'Yes' to confirm profiling
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new80.png)

91. Wait for profiling to complete by checking the notification icon (bell) located in the upper right hand corner.  You can also click the 'Refresh' icon on the right
<br> You can also click on the refresh icon on the right hand side
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new90.png)

92. Click on the 'Lineage'tab
<br>![](/exercises/ex2/images/DataPrep_Lineage_02_10_3new10.png)

93. Notice you can trace the lineage of the Customer_Sales_#.csv was created.  
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_Lineage_02_10_3new20.png)

may not need here to
***************
92. Click on 'Data Intelligence Metadata Explorer'
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_10_1new10.png)

93. Click 'Catalog'
<br>![](/exercises/ex2/images/DataPrep_Catalog_02_10_2new10.png)

94. Click 'Browse Connections'
<br>![](/exercises/ex2/images/DataPrep_Catalog_02_10_2new20.png)

95. Click 'DI_DATA_LAKE'
<br>![](/exercises/ex2/images/DataPrep_Catalog_02_10_2new30.png)

96. Click 'shared'
<br>![](/exercises/ex2/images/DataPrep_Catalog_02_10_2new40.png)

97. Click 'TechEd_DAT163_#'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_Catalog_02_10_2new50.png)

98. Click on the ellipsis (...) for 'Customer_Sales_#.csv'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_Catalog_02_10_2new60.png)

99. Click on 'New Publication'
<br>![](/exercises/ex2/images/DataPrep_Catalog_02_10_2new70.png)

100. Enter 'Customer_Sales_#' for publication name
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_Catalog_02_10_2new80.png)

101. Click 'Publish'
<br>![](/exercises/ex2/images/DataPrep_Catalog_02_10_2new90.png)

102. Click on the refresh icon on the top right to confirm your Customer_Sales_# is now published
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_Catalog_02_10_2new100.png)

*******************
to here

## Bind our new 'Customer_Sales" to our country rule

103. Click on 'Data Intelligence Metadata Explorer'
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_10_1new10.png)

104. Click on 'Rules'
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_10_2new10.png)

105. Click on 'View Rulebooks' from withing Rules
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_10.png)

106. Click on your 'TechEdDAT163_#'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_30.png)

107. Expand Accuracy rule category by clicking on the '>'
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_1new_10.png)

108. Click on the ellipsis (...) to the right under Rule Bindings
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_20.png)

109. Click on 'View Rule Bindings'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_30.png)

110. Click on the upper '+' in the upper right hand corner to Create a Rule Binding
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_40.png)

111. Click on the 'Browse' icon for 'Qualified Name'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_50.png)

112. Click on 'Browse' tab
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_60.png)

113. Click on the drop down arrow for 'Connections'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_70.png)

114. Select 'DI_DATA_LAKE'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_80.png)

115. Select on 'shared'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_90.png)

116. Select 'TechEd_DAT163_#'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_95.png)

117. Select 'Customer_Sales_#.csv'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_100.png)

118. Click 'OK'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_110.png)

119. Click 'Save'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_120.png)

120. Click 'Run All'
<br>![](/exercises/ex2/images/DataPrep_Rulebook_02_1new_130.png)

121. Click on 'Data Intelligence Metadata Explorer'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new10.png)

122. Click on 'Monitor'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new20.png)

123. Click on 'Monitor Tasks'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new30.png)

124. Notice your Rulebook is running
<br>![](/exercises/ex2/images/DataPrep_Monitor_02_10_1new10.png)

125. Wait for you Rulebook to Complete
<br>![](/exercises/ex2/images/DataPrep_Monitor_02_10_1new20.png)

126. Click on 'Data Intelligence Metadata Explorer'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new10.png)

127. Click on 'Rules'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new40.png)

128. Click on 'View Rulebooks'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new50.png)

129. Click on your 'TechEdDAT163_#'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_RuleBook_02_30.png)

130. Click on 'View Results'
<br>![](/exercises/ex2/images/DataPrep_RuleBookResults_02_1new10.png)

131. Click 'Yes' to view the updated Rule Results
<br>![](/exercises/ex2/images/DataPrep_RuleBookResults_02_2new10.png)

132. Notice your quality has improved from your Data Preparation
<br>![](/exercises/ex2/images/DataPrep_RuleBookResults_02_1new20.png)

133. Click on 'Data Intelligence Metadata Explorer'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new10.png)

134. Click on 'Rules'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new40.png)

135. Click on 'View Rules Dashboards'
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_10_1new10.png)

136.  'TechEd_DAT163_#'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_20.png)

137. Click on the pencil icon located on the right hand side
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_30.png)

138. Click on the '+' (plus sign) located next to your first dashboard
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_40.png)

139. Click on the drop down and select 'TechEd_DAT163_#'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_50.png)

140. Click on 'Step 2'
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_60.png)

141. Notice, 'Datasets is already selected; Click on 'Step 3'
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_70.png)

142. Select 'Single Dataset'
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_80.png)

143. Click on 'Step 4'
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_90.png)

144. Click on 'Select Customer_Sales_#'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_100.png)

145. Click on 'Step 5'
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_110.png)

146. Click on 'Save'
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_120.png)

147. You have now created a new dashboard for your combined Customer and Sales file
<br>![](/exercises/ex2/images/DataPrep_Dashboard_02_1new_130.png)






************************

END HERE


148. Click on 'Data Intelligence Metadata Explorer'
<br>![](/exercises/ex2/images/DataPrep_DIMenu_02_10_1new10.png)

149. Select 'Home'
<br>![](/exercises/ex2/images/DataPrep_DIMenuHome_02_10_1new10.png)

150. Click 'View Preparations'
<br>![](/exercises/ex2/images/DataPrep_ViewPreo_02_10_1new10.png)

151. Click on 'Customer_Sales_#'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new20.png)

152. Select 'Actions'
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new30.png)

153. Select 'Manage Preparation Tasks'
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new40.png)

154. Click on the ellipsis (...) for 'Customer_Sales_#.csv'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new50.png)

155. Select 'View Fact Sheet'
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new60.png)

156. Start Profiling by clicking in the Run icon on the right hand side
<br>![](/exercises/ex2/images/DataPrep_ViewPrep_02_10_1new70.png)



## Summary

You've now successfully discovered data, defined a rule based on your profiling results and to check the quality of data, create a glossary term to associate with your data, used self-service data preparation to correct the data, aggregated the sales data to understand how much each customer has bought from you, created a dashboard to monitor the quality of your data as well as watch the trend of your data.

Continue to - [Exercise 3 - Excercise 3 ](../ex3/README.md)
