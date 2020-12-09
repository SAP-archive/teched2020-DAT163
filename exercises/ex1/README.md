After completing these steps you will have created adding a rule and a dashboard

# Objective

As a Data Steward you need to be able to define rules and build dashboards to monitor the quality of the data and view the trend of the data quality.   In this exercise, we will create data quality rule and monitor the data quality of the data.

## Create Data Quality Rule

1. Click on 'Data Intelligence Metadata Explorer drop down
<br>![](/exercises/ex1/images/Rules_DI_MM_DropDown_01_10new.png)

2. Click on Rules
<br>![](/exercises/ex1/images/Rules_DI_MM_DropDown_01_10new_2new.png)

3. Click 'View Rules' 
<br>![](/exercises/ex1/images/Rules_DI_MM_DropDownRules_01_10.png)

4. Notice the existing Rule Categories, highlighted in blue
<br>![](/exercises/ex1/images/Rules_ViewRules_01_10.png)

5. We want to create a rule to check that the country code contains only the value 'US', since this is a US file.  For the Rule Category Accuracy, Click on the Create Rule icon (folder with a plus sign) to the right of the Accuracy rule category
<br>![](/exercises/ex1/images/Rules_NewRule_01_100_2new.png)

6. For Rule ID, enter 'Country US_#'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex1/images/Rules_Create_01_100.png)

7. For Name, enter 'Country US_#'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex1/images/Rules_Create_01_110.png)

8. For Description, enter 'The US customer file must not be null and must have a standardized country value of 'US', for Group #.'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex1/images/Rules_Create_01_120.png)

9. Click 'Save'
<br>![](/exercises/ex1/images/Rules_Create_01_130.png)

10. Click on the '+' for the Add a Parameter on the right hand side
<br>![](/exercises/ex1/images/Rules_Create_01_140.png)

11. For Name, enter in 'Country'
<br>![](/exercises/ex1/images/Rules_Create_01_150.png)

12. Click on the Save icon, located on the right
<br>![](/exercises/ex1/images/Rules_Create_01_160.png)

13. Add Condition, by clicking on the '+' on the right of the Conditions row
<br>![](/exercises/ex1/images/Rules_Create_01_170.png)

14. For Condition Name, enter 'CountryNotNull'
<br>![](/exercises/ex1/images/Rules_Create_01_180.png)

15. For Parameter Name, click on the drop down 
<br>![](/exercises/ex1/images/Rules_Create_01_190.png)

16. Select 'Country'
<br>![](/exercises/ex1/images/Rules_Create_01_200.png)

17. The Operator is by default set to 'is not null'
<br>![](/exercises/ex1/images/Rules_Create_01_210.png)

18. Add another condition, by clicking on the '+' on the right of the Conditions row
<br>![](/exercises/ex1/images/Rules_Create_01_220.png)

19. For Condition2 Name, enter 'CountryUS'
<br>![](/exercises/ex1/images/Rules_Create_01_230.png)

20. For Parameter Name, click on the drop down 
<br>![](/exercises/ex1/images/Rules_Create_01_240.png)

21. Select 'Country'
<br>![](/exercises/ex1/images/Rules_Create_01_250.png)

22. For Operator, click on the drop down
<br>![](/exercises/ex1/images/Rules_Create_01_260.png)

23. Select 'equals'
<br>![](/exercises/ex1/images/Rules_Create_01_267.png)

24. For Value or Format, enter 'US'
<br>![](/exercises/ex1/images/Rules_Create_01_270.png)

25. Click on the Save icon for Conditions
<br>![](/exercises/ex1/images/Rules_Create_01_280.png)

26. In the upper right hand corner click on 'Test Rule'
<br>![](/exercises/ex1/images/Rules_DefinitionExpand_01_10.png)

27. Click on the '+' to add a country code to test
<br>![](/exercises/ex1/images/Rules_TestAddRecord_01_10.png) 

28. Enter 'US' in country parameter where you see 'Enter value'
<br>![](/exercises/ex1/images/Rules_TestAddRecord1_01_100.png)

29. Click on the '+' to add another country to test 
<br>![](/exercises/ex1/images/Rules_TestAddRecord1_01_110.png) 

30. Enter 'USA' in country parameter where you see 'Enter value'
<br>![](/exercises/ex1/images/Rules_TestAddRecord1_01_120.png)

31. Click on the '+' to add another country to test 
<br>![](/exercises/ex1/images/Rules_TestAddRecord1_01_110.png) 

32. Enter 'U.S.A.' in country parameter where you see 'Enter value'
<br>![](/exercises/ex1/images/Rules_TestAddRecord1_01_130.png)

33. Click on the '+' to add another country to test 
<br>![](/exercises/ex1/images/Rules_TestAddRecord1_01_110.png) 

34. Enter 'U.S.' in country parameter where you see 'Enter value'
<br>![](/exercises/ex1/images/Rules_TestAddRecord1_01_140.png)

35. Click on 'Run Test'
<br>![](/exercises/ex1/images/Rules_TestAddRecordsResults_01_10.png)

36. Notice only the first record of 'US' shows rules that it passed the rule conditions.
<br>![](/exercises/ex1/images/Rules_CloseTestRules_01_10.png)

37. Click on 'Data Intelligence Metadata Explorer' drop down at the top of the screen 
<br>![](/exercises/ex1/images/Rules_DIDropDown_01_10.png)

38. Select 'View Rulebooks' 
<br>![](/exercises/ex1/images/Rules_DIDropDown_01_110.png)

39. Click on the '+' in the upper right hand corner to Create a Rulebook
<br>![](/exercises/ex1/images/Rules_CreateRulebook_01_10.png)

40. On the right hand side enter 'TechEd_DAT163_#' for Name 
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex1/images/Rules_CreateTechedRulebook_01_10.png)

41. For Description, enter 'TechEd DAT163 Group #' 
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex1/images/Rules_CreateTechedRulebook_01_110.png)

42. Click 'Save' at the bottom right hand corner
<br>![](/exercises/ex1/images/Rules_SaveRulebook_01_10.png)

43. Click the Import Rules icon on the right hand side
<br>![](/exercises/ex1/images/Rules_ImportRulesToRulebook_01_10.png)

44. Expand 'Accuracy', by clicking on '>'
<br>![](/exercises/ex1/images/Rules_ExpandConformity_01_10.png)

45. Select the rule you created, 'Country US_#'
<br>Note: where # is the number assigned to you 
<br>![](/exercises/ex1/images/Rules_Country_01_10.png)

46. Click 'Save
<br>![](/exercises/ex1/images/Rules_SavePostcode5ToRulebook_01_10.png)

47. Notice the the Rulebook you created doesn't contain any rule bindings
<br>![](/exercises/ex1/images/Rules_NoBindDatasets_01_10.png)

48.  Click on the ... (elipsis / 3 dots) to the right of Country
<br>![](/exercises/ex1/images/Rules_BindPostCode5_01_10.png)

49. Click on 'View Rule Bindings'
<br>![](/exercises/ex1/images/Rules_ViewRuleBinding_01_10.png)

50. Click on the '+' sign to Create a Rule Binding
<br>![](/exercises/ex1/images/Rules_AddRuleBindDatasets_01_10.png)

51. Click on the browse icon for the Qualified Name parameter
<br>![](/exercises/ex1/images/Rules_QualifiedName_01_10.png)

52. Click on the drop down for 'Select a connection and select 'DI_DATA_LAKE'
<br>![](/exercises/ex1/images/Rules_SelectDIDataLake_01_10.png)

53. Click on 'shared'
<br>![](/exercises/ex1/images/Rules_ExpandShared_01_10.png)

54. Click on 'TechEd_DAT163_#'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex1/images/Rules_ExpandShared_01_110.png)

55. Select 'Customer_US2_#.parquet' 
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex1/images/RUles_SelectCustomerParquet_01_10.png)

56. Click 'OK'
<br>![](/exercises/ex1/images/Rules_CLickOK_01_10.png)

57. Click 'Save' in the bottom right hand corner
<br>![](/exercises/ex1/images/Rules_SaveRuleBinding_01_10.png)

Congratulations, you have now bound the rule you created (Country US) to your Customer parquet dataset, 

## Run the rule against the dataset

58. Click 'Run All'
<br>![](/exercises/ex1/images/Rule_RunAll_01_10.png)

59. Click on 'Data Intelligence Metadata Explorer' drop down 
<br>![](/exercises/ex1/images/Rules_checkMonitor_01_10.png)

60. Select 'Monitor'
<br>![](/exercises/ex1/images/Rules_checkMonitor_01_110.png)

61. Click on 'Monitor Tasks' 
<br>![](/exercises/ex1/images/Rules_checkMonitor_01_120.png)

62. Find your rule task name and number (TechEd_DAT163_#)
<br>Note: replace # with the number assigned to you
<br>If it says 'Completed' the rule execution is complete.  Note: this is another way to check the status of your task; you will still see when it is started an completed with the Notificiation icon in the upper right hand corner.
<br>![](/exercises/ex1/images/RUle_completed_01_10.png)

63. Click on 'Data Intelligence Metadata Explorer' dropdown 
<br>![](/exercises/ex1/images/Rules_Monitor_DIMain_01_10.png)

64. Select 'Rules'
<br>![](/exercises/ex1/images/Rules_Monitor_DIMain_01_20.png)

65. Click on 'View Rulebooks' 
<br>![](/exercises/ex1/images/Rule_ViewRulebooks_01_10.png)

66. In the search window type in '#', this is helpful when you have multiple Rulebooks.
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex1/images/Rules_SearchFindRulebook_01_10.png)

67. Click on your TechEd Rulebook, 'TechEdDAT163_#
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex1/images/Rules_SelectYourRulebook_01_10.png)

68. Click on 'View Results'
<br>![](/exercises/ex1/images/Rule_ViewResults_01_10.png)

69. Notice 78.72% of the records passed our Country US rule.
<br>![](/exercises/ex1/images/Rule_ExpandResults_01_20.png)

70. Expand 'Dataset: Customer_US2_#.parquet' by clicking on the '>' icon
<br>Note: where # is the number assigned to you
<br>![](/exercises/ex1/images/Rule_ExpandResults_01_120.png)

71. You can see the parquet file contains 329 records and 259 records passed the Country US rule.
<br>![](/exercises/ex1/images/Rule_ExpandResults_01_130.png)

72. Click 'View Failed Rows' on the right hand side of 'Rule: Country US
<br>![](/exercises/ex1/images/Rule_FailedRecords_01_140.png)

73. Notice the Country column shows records that are USA, U.S.A., U.S., and null
<br>![](/exercises/ex1/images/Rules_FailedRecResults_01_150.png)


## Create a Data Quality Dashboard

74. Click on 'Data Intelligence Metadata Explorer' drop down 
<br>![](/exercises/ex1/images/Rules_DIMain_FailRec_01_10.png)

75. Click on 'View Rules Dashboards'
<br>![](/exercises/ex1/images/Rules_GoToDashboard_01_10.png)

76. Click on the '+' to Create a Dashboard
<br>![](/exercises/ex1/images/Rules_CreateDashboard_01_10.png)

77. For Name, enter 'TechEd_DAT163_#'
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_20.png)

78. For Description, enter 'Dashboard for TechEdDATA for Group #' 
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_120.png)

79. Click Save
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_130.png)

80. Click on the '+' to add scorecard
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_150.png)

81. Click the dropdown for 'Select a rulebook'
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_30.png)

82. Select your TechEdDAT163_#
<br>Note: replace # with the number assigned to you
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_160.png)

83. Click 'Step 2'
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_40.png)

84. Confirm you want to report on the 'Datasets' and that it is already selected.  Click 'Step 3'
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_50.png)

85. Select 'Single Dataset' 
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_60.png)

86. Select on 'Pass %'
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_70.png)

87. Click 'Step 4'
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_80.png)

88. Click on 'Select a dataset' dropdown
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_90.png)

89. Select 'Customer_US2_#.parquet'
<br>Note: where # is the number assigned to you
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_92.png)

90. Click 'Step 5'
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_100.png)

91. Click 'Save' 
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_110.png)

92. Notice your Dashboard has been created
<br>![](/exercises/ex1/images/Rules_DashboardResultsCreate_01_110.png) 

FYI - if you had choosen to create your rulebook based on score instead of % your dashboard would have looked like:
<br>![](/exercises/ex1/images/Rules_DashboardResultsCreate_01_120.png)



## Summary

You have completed defining a rule, binding the rule, creating a rulebook and a dashboard to reflect the quality of your data.  Continue to - [Exercise 3 - Search, Self-Service Data Preparation, Review Results, and Lineage](../ex2/README.md)

