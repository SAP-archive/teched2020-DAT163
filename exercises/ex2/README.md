# Exercise 2 - Exercise 2 Description

In this exercise, we will create...

## Exercise 2.1 Sub Exercise 1 Description

After completing these steps you will have created...

1. Click on the 'Data Intelligence Metadata Explorer' drop down and select 'Home'
<br>![](/exercises/ex2/images/DataPrep_DI_MM_Home_02_10.png)

2.	Select 'Browse the Catalog'
DataPrep_DI_MM_BrowseCat_02_10.png)

3. Enter '##' in the Search entire catalog text box
where ## is the group number assigned to you
DataPrep_DI_SearchCat_02_10.png)

4. Hover over your 'Customers_US2.parquet##' file and click on the glasses icon to view the factsheet
where ## is the group number assigned to you
DataPrep_CustomersFactsheet_02_10.png)

5. Click on the 'Country' column name and notice on the right hand side the distinct values in this column are 'US', 'U.S.A.', 'USA', 'U.S.', and nulls.  This dataset is for US and the country column should have the same value for all the records.
DataPrep_FactSheet_DistinctValue_02_10.png)

6. Click on the comments and notice one of them states that the name not broken out into First Name and Last Name as is your organizational standards, but instead is to have one full name column
DataPrep_Comments_02_10.png)

7. Close the Comments window
DataPrep_CloseComments_02_10.png)

8. Click on'Prepare Data'
DataPrep_StartPrep_02_10.png)

9. Click the 'Country' column
DataPrep_SelectCountryCol_02_10.png)

10. Click on 'Replace'
DataPrep_SelectCountryReplace_02_10.png)

11. Your organization's standard is for the US country values to be 'USA'.  For Replace leave the Search on 'Custom String'
Enter the search value as 'U.S.A'
For Replace by, enter 'USA'
DataPrep_SelectCountryReplace_02_20.png)

12. Find one of the rows in country that has U.S.A 
DataPrep_SelectCountryReplace_02_25.png)

13. Click 'Apply'
DataPrep_SelectCountryReplace_02_30.png)

13. Look at the same record and notice the country now says 'USA'
DataPrep_SelectCountryReplace_02_40.png)

14. Click on 'Replace'
DataPrep_SelectCountryReplace_02_10.png)

15. Continue replacing country values with your organization's standard of 'USA'.  For Replace leave the Search on 'Custom String'
Enter the search value as 'US'
For Replace by, enter 'USA'
DataPrep_SelectCountryReplace_02_45.png)

16. Click 'Apply'
DataPrep_SelectCountryReplace_02_30.png)

17. Click on 'Replace'
DataPrep_SelectCountryReplace_02_10.png)

18. Continue replacing country values with your organization's standard of 'USA'.  For Replace leave the Search on 'Custom String'
Enter the search value as 'USAA'
For Replace by, enter 'USA'
DataPrep_SelectCountryReplace_02_50.png)

19. Click 'Apply'
DataPrep_SelectCountryReplace_02_30.png)

20. Click on 'Replace'
DataPrep_SelectCountryReplace_02_10.png)

21. Continue replacing country values with your organization's standard of 'USA'.  For Replace leave the Search on 'Custom String'
Enter the search value as 'U.S.
For Replace by, enter 'USA'
DataPrep_SelectCountryReplace_02_7.png)

22. Click 'Apply'
DataPrep_SelectCountryReplace_02_30.png)

23. Click on 'Replace'
DataPrep_SelectCountryReplace_02_10.png)

24. Replace the 'null' values in the country column with with your organization's standard of 'USA'.  For change Search to 'NULL'
For Replace by, 
   Select 'Custom String'
   Value enter 'USA'
DataPrep_SelectCountryReplace_02_60.png)

25. Click 'Apply'
DataPrep_SelectCountryReplace_02_30.png)

26. Look at the Country column and notice all the values are standardized and consistent with 'USA'
DataPrep_SelectCountryReplace_02_80.png)

27. Your organizational standard is also to have one address line and this dataset has three, so we will combine them so we have one address column, without losing any data.
Click on the 'Address1' column
DataPrep_AddressPrep_02_10.png)

28. Click 'Combine' on the right hand side
DataPrep_AddressPrep_02_20.png)

29. Click on 'Address2'
DataPrep_AddressPrep_02_30.png)

30. Click on 'Address3'
DataPrep_AddressPrep_02_40.png)

31. For Combine using: enter a ' ' (space) for the Separator
DataPrep_AddressPrep_02_50.png)

32. For New Column Name* enter 'Full_Address'
DataPrep_AddressPrep_02_60.png)

33. Click Apply
DataPrep_AddressPrep_02_70.png)

34. After 'Address3' column you will now see your new 'Full_Address' column that now contains the complete address
DataPrep_AddressPrep_02_80.png)

## 35. You also want to fix the name so you have the complete name in one column.  Click on First_name
## DataPrep_FullNamePrep_02_10.png)

## 36. Click 'Split' on the right hand side
## DataPrep_FullNamePrep_02_30.png)

## 37. Enter a ' ' (space) for separater
## DataPrep_FullNamePrep_02_40.png)

## 38. Enter 'FirstName' for Column 1 name
## DataPrep_FullNamePrep_02_50.png)

## 39. Enter 'LastName' for Column 2 name
## DataPrep_FullNamePrep_02_60.png)

## 40. Click 'Apply'
## DataPrep_FullNamePrep_02_70.png)

## 41. Notice after 'FullName' you now have a discrete 'FirstName' and 'LastName'



##
## Is there a way to Save my data set changes?
##


35. Click on the 'Data Intelligence Metadata Explorer' drop down
DataPrep_DI_DropDown_02_10.png)

36. Select 'Browse Catalog'
DataPrep_DI_DropDowBrowse_Catalog_02_10.png)

37. Enter 'sales*' in the Search entire catalog text box
DataPrep_SearchCatalog_02_10.png)

38. Select '...' on your 'Sales_data_##.csv' 
where ## is the group number assigned to you
DataPrep_SalesData_02_05.png)

39. Choose 'Prepare Data'
DataPrep_SalesData_02_10.png)

40. Notice the sales data has 'TRANS_ID', 'CUST_ID', 'TRANS_AMT', and 'TRANS_DATE', but you cannot see the customer details, such as name, address, and so on.  Click on the 'Actions' on the right hand side.
DataPrep_SalesData_02_20.png)

41. Select 'Enrich Preparation'
DataPrep_ActionJoin_02_10.png)

37. You want to do a Left Outer Join, which will includes all rows from the both datasets, where a inner join would only include matching rows from the datasets.  Select 'Customers_US2_##'
where ## is the group number assigned to you
DataPrep_ActionJoin_02_30.png)

38. Drag 'Customers_US2_##' to the left hand side tile that says 'Drop here to merge'
where ## is the group number assigned to you
DataPrep_ActionJoin_02_40.png)

39. Select 'Left Join
DataPrep_ActionJoin_02_50.png)

40. Change 'TRANS_ID' to 'CUST_ID'.  This will allow you to join the two datasets on the common column of customer id.
DataPrep_ActionJoin_02_60.png)

41. Click 'Apply'
DataPrep_ActionJoin_02_70.png)

42. Scroll to the right and notice the customer data now has 'TRANS_ID', 'CUST_ID', 'TRANS_AMT', and 'TRANS_DATE' data associated to it.
DataPrep_ActionJoin_02_80.png)

43. Click 'Apply Enrichment'
DataPrep_ActionJoin_02_90.png)

44. 









## Summary

You've now ...

Continue to - [Exercise 3 - Excercise 3 ](../ex3/README.md)
