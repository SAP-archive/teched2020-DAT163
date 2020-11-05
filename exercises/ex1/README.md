After completing these steps you will have created adding a rule

# Exercise 1 - Exercise 1 Description

In this exercise, we will create data quality rule and monitor the data quality of your data.

## Exercise 1.1 Sub Exercise 1 Description

1. If in the Catalog from Ex0, click on the drop down of 'Data Intelligence Metadata Explorer' and Click on Rules
<br>![](/exercises/ex1/images/Rules_DI_MM_DropDown_01_10.png)

2. Click 'View Rules' 
<br>![](/exercises/ex1/images/Rules_DI_MM_DropDownRules_01_10.png)

3. Notice the existing Rule Categories
<br>![](/exercises/ex1/images/Rules_ViewRules_01_10.png)

4. Enter 'post' in the 'Filter rule names' parameter
<br>![](/exercises/ex1/images/Rules_Search_01_10.png)

5. Expand 'Conformity (1) 
   Click on the '>' (Rule Details) for the USPostalCodeConformityRule on the right hand side
<br>![](/exercises/ex1/images/Rules_SearchConformity_01_10.png)

6. Under Pameters you will notice it is looking at a 'Zipcode' column that is an Integer data type
<br>![](/exercises/ex1/images/Rules_Definition_01_10.png)

7. Expand 'Condition' and note that the condition of the rule is checking that the zipcode is not null and that the zipcode has a 5 digit number
<br>![](/exercises/ex1/images/Rules_DefinitionExpand_01_10.png)

8. Go back to Rule Overview, by clicking on the '<' Next to Rule Definition
<br>![](/exercises/ex1/images/Rules_DefinitionExpand_01_110.png)

9. We want to check if the country has the standard value of 'US' since this is a US only customer file.  Enter 'country' for Filter rule names
<br>![](/exercises/ex1/images/Rules_Search_01_100.png)

10. Press the Enter key or click on the magnifying glass to search for country
<br>![](/exercises/ex1/images/Rules_Search_01_110.png)

11. No results for country are found. We will add a country rule to check that country is 'US' only.  Click on the Create Rule icon in the Accuracy's Rule Category on the right hand.
<br>![](/exercises/ex1/images/Rules_Search_01_120.png)

12. For Rule ID, enter 'Country US' 
<br>![](/exercises/ex1/images/Rules_Create_01_100.png)

13. For Name, enter 'Country US'
<br>![](/exercises/ex1/images/Rules_Create_01_110.png)

14. For Description, enter 'The US customer file must not be null and must have a standardized country value of 'US'.'
<br>![](/exercises/ex1/images/Rules_Create_01_120.png)

15. Click 'Save'
<br>![](/exercises/ex1/images/Rules_Create_01_130.png)

16. Click on the '+' for the Add a Parameter on the right hand side
<br>![](/exercises/ex1/images/Rules_Create_01_140.png)

17. For Name, enter in 'Country'
<br>![](/exercises/ex1/images/Rules_Create_01_150.png)

18. Click on the Save icon, located on the right
<br>![](/exercises/ex1/images/Rules_Create_01_160.png)

19. Add Condition, by clicking on the '+' on the right of the Conditions row
<br>![](/exercises/ex1/images/Rules_Create_01_170.png)

20. For Condition Name, enter 'CountryNotNull'
<br>![](/exercises/ex1/images/Rules_Create_01_180.png)

21. For Parameter Name, click on the drop down 
<br>![](/exercises/ex1/images/Rules_Create_01_190.png)

22. Select 'Country'
<br>![](/exercises/ex1/images/Rules_Create_01_200.png)

23. The Operator is by default set to 'is not null'
<br>![](/exercises/ex1/images/Rules_Create_01_210.png)

24. Add another condition, by clicking on the '+' on the right of the Conditions row
<br>![](/exercises/ex1/images/Rules_Create_01_220.png)

25. For Condition2 Name, enter 'CountryUS'
<br>![](/exercises/ex1/images/Rules_Create_01_230.png)

21. For Parameter Name, click on the drop down 
<br>![](/exercises/ex1/images/Rules_Create_01_240.png)

22. Select 'Country'
<br>![](/exercises/ex1/images/Rules_Create_01_250.png)

23. For Operator, click on the drop down
<br>![](/exercises/ex1/images/Rules_Create_01_260.png)

24. Select 'equals'
<br>![](/exercises/ex1/images/Rules_Create_01_267.png)

25. For Value or Format, enter 'US'
<br>![](/exercises/ex1/images/Rules_Create_01_270.png)

26. Click on the Save icon for Conditions
<br>![](/exercises/ex1/images/Rules_Create_01_280.png)







8. In the upper right hand corner click on 'Test Rule'
<br>![](/exercises/ex1/images/Rules_DefinitionExpand_01_10.png)

9. Click on the '+' to add a zipcode to test
<br>![](/exercises/ex1/images/Rules_TestAddRecord_01_10.png) 

10. Enter '54601' in zipcode parameter where you see 'Enter value'
<br>![](/exercises/ex1/images/Rules_TestAddRecord1_01_10.png)

11. Click on the '+' to add another zipcode to test and add '123456'
<br>![](/exercises/ex1/images/Rules_TestAddRecord2_01_10.png) 

(UPDATE: Remove if I can't edit a rule)
12. Click on the '+' to add another zipcode to test and add '123'
<br>![](/exercises/ex1/images/Rules_TestAddRecord3_01_10.png) 

13. Click on 'Run Test'
<br>![](/exercises/ex1/images/Rules_TestAddRecordsResults_01_10.png)

14. Notice only the second record of '123456' fails.  So we need to modify the zipcode rule so that only 5 digit zipcodes pass.  (MAY Delete if i can't modify an existing rule) Click on the '<' next to Test Cases to take us back to the Rule Definition  
<br>![](/exercises/ex1/images/Rules_CloseTestRules_01_10.png)

15. CLick on the (MAY Delete if i can't modify an existing rule) 
<br>![](/exercises/ex1/images/Rules_DefinitionExpand_01_10.png)

16. Click on the Create a Rule icon (icon: list with a +) on the right hand side of the Conformity Rule Category to add a new rule
<br>![](/exercises/ex1/images/Rules_AddARule_01_10.png)

17. Enter 'PostCode5' for the Rule ID., ' Name and 'US PostCode 5' for Name, and  'US Postal Code must be 5 digits long' for Description
<br>![](/exercises/ex1/images/Rules_AddRuleNameDesc_01_10.png)

18. Click Save
<br>![](/exercises/ex1/images/Rules_AddRuleNameDesc_01_10.png)

19. Click the '+' to the right of Parameters 
<br>![](/exercises/ex1/images/Rules_AddARuleParameter_01_10.png)

20. Enter 'Zipcode' for the Name, Select 'Integer' for the Type' and click the Save icon
<br>![](/exercises/ex1/images/Rules_SaveParameter_01_10.png)

21. Expand Condition and click the '+' to the right of Conditions
<br>![](/exercises/ex1/images/Rules_AddExpandCondition_01_10.png)

22. Enter 'ValueCheck2' for Condition Name, 
    Enter 'Zipcode' for Parameter Name, 
    Select 'is between' for Operator,
    Select 'User Entry' for Mode, and
    Enter in '10000' for from and '99999' for to in Value or Format parameter
<br>![](/exercises/ex1/images/Rules_NewPostcode5_01_10.png)

23. Expand Condition and click the '+' to the right of Conditions
<br>![](/exercises/ex1/images/Rules_AddExpandCondition_01_10.png)

24. Enter 'NotEmpty' for Condition Name, 
    Enter 'Zipcode' for Parameter Name, and
    Select 'is not null' for Operator
<br>![](/exercises/ex1/images/Rules_AddCondition2_01_10.png)

25. Click the save icon on the right hand side of Conditions
<br>![](/exercises/ex1/images/Rules_ConditionSave_01_10.png)

8. In the upper right hand corner click on 'Test Rule'
<br>![](/exercises/ex1/images/Rules_DefinitionExpand_01_10.png)

13. Verify your same test records are still there and then click on 'Run Test'
<br>![](/exercises/ex1/images/Rules_TestAddRecordsResults_01_10.png)

14. Notice only the first record of '54601' passes.  Both the test zipcodes of '123456' and '123' fail.  
<br>![](/exercises/ex1/images/Rules_TestResults2_01_10.png)

15. Click on 'Data Intelligence Metadata Explorer' at the top of the screen and select 'View Rulebooks' under rules
<br>![](/exercises/ex1/images/Rules_DIDropDown_01_10.png)

16. CLick on the '+' in the upper right hand corner to Create a Rulebook
<br>![](/exercises/ex1/images/Rules_CreateRulebook_01_10.png)

17. On the right hand side enter TechEdDAT163_## for Name and 'TechEd DAT163 Group ##' for Description
Note: replace ## with the nummber assigned to you
<br>![](/exercises/ex1/images/Rules_CreateTechedRulebook_01_10.png)

18. Click 'Save' at the bottom right hand corner
<br>![](/exercises/ex1/images/Rules_SaveRulebook_01_10.png)

19. Click the Import Rules icon on the right hand side
<br>![](/exercises/ex1/images/Rules_ImportRulesToRulebook_01_10.png)

20. Expand 'Conformity'
<br>![](/exercises/ex1/images/Rules_ExpandConformity_01_10.png)

21. Select the rule you created, 'PostCode5'
<br>![](/exercises/ex1/images/Rules_PostCode5_01_10.png)

22. Click 'Save
<br>![](/exercises/ex1/images/Rules_SavePostcode5ToRulebook_01_10.png)

23. Notice the the Rulebook you created doesn't contain rules that are boud to any datasets
<br>![](/exercises/ex1/images/Rules_NoBindDatasets_01_10.png)

24.  Click on the 3 elipsis to the right of PostCode5
<br>![](/exercises/ex1/images/Rules_BindPostCode5_01_10.png)

25. Click on 'View Rule Bindings'
<br>![](/exercises/ex1/images/Rules_ViewRuleBinding_01_10.png)

26. CLick on the '+' signe to Create a Rule Binding
<br>![](/exercises/ex1/images/Rules_AddRuleBindDatasets_01_10.png)

27. Click on the select a dataset icon on the right
<br>![](/exercises/ex1/images/Rules_Qualified Name_01_10.png)

28. Click on the drop down for 'Select a connection and select 'DI_DATA_LAKE'
<br>![](/exercises/ex1/images/Rules_SelectDIDataLake_01_10.png)

29. Expand Shared
<br>![](/exercises/ex1/images/Rules_ExpandShared_01_10.png)

30. Select 'Customer_US2.parquet' 
<br>![](/exercises/ex1/images/RUles_SelectCustomerParquet_01_10.png)

31. Click 'OK'
<br>![](/exercises/ex1/images/Rules_CLickOK_01_10.png)

32. Click 'Save in the bottom right hand corner
<br>![](/exercises/ex1/images/Rules_SaveRuleBinding_01_10.png)

Congratulations, you have now bound the rule you created (PostCode5) to your Customer dataset, now let's run the rule against the dataset.

33. Click 'Run All'
<br>![](/exercises/ex1/images/Rule_RunAll_01_10.png)

34. Click on 'Data Intelligence Metadata Explorer' drop down and select 'Monitor'
<br>![](/exercises/ex1/images/Rules_checkMonitor_01_10.png)

35. Click on 'Monitor Tasks' 
<br>![](/exercises/ex1/images/Rules_checkMonitor_01_10.png)

36. At the top of the task list will be your rule running.  If it says 'Completed' it is the rule execution is complete
<br>![](/exercises/ex1/images/RUle_completed_01_10.png)

37. Click on 'Data Intelligence Metadata Explorer' drop down and select 'Rules'
<br>![](/exercises/ex1/images/Rule_Select Rules_01_10.png)

35. Click on 'View Rulebooks' 
<br>![](/exercises/ex1/images/Rule_ViewRulebooks_01_10.png)

36. In the search window type in 'tech' and notice your Rulebook in the Rulebook
<br>![](/exercises/ex1/images/Rules_SearchFindRulebook_01_10.png)

37. Click on your TechEd Rulebook ('TechEdDAT163_##)
<br>![](/exercises/ex1/images/Rules_SelectYourRulebook_01_10.png)

38. Click on 'View Results'
<br>![](/exercises/ex1/images/Rule_ViewResults_01_10.png)

39. Notice 91.49% of the records passed our zipcode is 5 digit rule.
You can also see that there were 301 records on input.
Expand 'Dataset: Customer_US2_##.parquet'
Note: where ## is the number assigned to you
<br>![](/exercises/ex1/images/Rule_ExpandResults_01_20.png)

40. Click 'View Failed Rows' on the right hand side of 'Rule: US PostCode5
<br>![](/exercises/ex1/images/Rule_FailedRecords_01_10.png)

41. Scroll to the righ until you gets to the 'ZipCode' column. Notice the zipcodes that failed are only 4 digits in length and not the 5 needed and one of the records is 'null'
<br>![](/exercises/ex1/images/Rules_FailedRecResults_01_10.png)

42. Click on 'View Rules Dashboards' from 'Data Intelligence Metadata Explorer' drop down
<br>![](/exercises/ex1/images/Rules_GoToDashboard_01_10.png)

43. Click on the '+' to Create a Dashboard
<br>![](/exercises/ex1/images/Rules_CreateDashboard_01_10.png)

44. Enter 'TechEdDATA_##' for Name and a Description of 'Dashboard for TechEdDATA for Group 07' and 
Click Save
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_10.png)

45. Click on the '+' to add scorecard
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_20.png)

46. Click the dropdown for 'Select a rulebook'
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_30.png)

47. Select your TechEdDAT163_##
Note: where ## is the number assigned to you
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_30.png)

48. Click 'Step 2'
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_40.png)

49. Confirm you want to report on the 'Datasets' and that it is already selected.  Click 'Step 3'
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_50.png)

50. Select 'Single Dataset' 
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_60.png)

51. Select on 'Pass %'
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_70.png)

52. Click 'Step 4'
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_80.png)

53. Click on 'Select a dataset' dropdown
Select 'Customer_US2_##.parquet'
Note: where ## is the number assigned to you
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_90.png)

54. Click 'Step 5'
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_100.png)

55. Click 'Save' 
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_110.png)

56. Notice your Dashboard has been created
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_120.png) 

FYI if you had choosen to create your rulebook based on score instead of % your dashboard would have looked like:
<br>![](/exercises/ex1/images/Rules_DashboardCreate_01_130.png)

## Summary

You've now ...

Continue to - [Exercise 2 - Exercise 2 Description](../ex2/README.md)

