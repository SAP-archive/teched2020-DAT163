# Exercise 1 - Exercise 1 Description

In this exercise, we will create data quality rule and monitor the data quality of your data.

## Exercise 1.1 Sub Exercise 1 Description

1. If in the Catalog from Ex0, click on the drop down of 'Data Intelligence Metadata Explorer' and Click on Rules
<br>![](/exercises/ex1/images/Rules_DI_MM_DropDown_01_10.png)

2. CLick 'View Rules' 
<br>![](/exercises/ex1/images/Rules_DI_MM_DropDownRules_01_10.png)

After completing these steps you will have created adding a rule

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





After completing these steps you will have created adding a rule

1. Click here.
<br>![](/exercises/ex1/images/01_01_0010.png)

2.	Insert this line of code.
```abap
response->set_text( |Hello World! | ). 
```



## Exercise 1.2 Sub Exercise 2 Description

After completing these steps you will have...

1.	Enter this code.
```abap
DATA(lt_params) = request->get_form_fields(  ).
READ TABLE lt_params REFERENCE INTO DATA(lr_params) WITH KEY name = 'cmd'.
  IF sy-subrc <> 0.
    response->set_status( i_code = 400
                     i_reason = 'Bad request').
    RETURN.
  ENDIF.

```

2.	Click here.
<br>![](/exercises/ex1/images/01_02_0010.png)


## Summary

You've now ...

Continue to - [Exercise 2 - Exercise 2 Description](../ex2/README.md)

