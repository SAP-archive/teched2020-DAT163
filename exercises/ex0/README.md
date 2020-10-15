# Level 1 Heading

In this exercise, you will upload datasets, proflie the data, create a relationship with data and a glossary term
(UPDATE add more)

## Level 2 Heading

After completing these steps you will have logged into SAP Data Intellegence

1.	Open Chrome and go to (UPDATE add URL)
<br>![](/exercises/ex0/images/LogOn_Default_00_10.jpg)

2.	Insert this code.
```
 DATA(lt_params) = request->get_form_fields(  ).
 READ TABLE lt_params REFERENCE INTO DATA(lr_params) WITH KEY name = 'cmd'.
  IF sy-subrc <> 0.
    response->set_status( i_code = 400
                     i_reason = 'Bad request').
    RETURN.
  ENDIF.
```

## Summary

Now that you have ... 
Continue to - [Exercise 1 - Exercise 1 Description](../ex1/README.md)
