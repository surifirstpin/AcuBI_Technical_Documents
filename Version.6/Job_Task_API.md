

<h1><center>Job Task Type (API)</center> </h1>

  


 Functionality :  </b>

Application Programming interface (‘API’) is a computing interface that defines interactions between multiple software intermediaries.This feature allows to extract data stored in the form of an xml in the given API as data columns and allows to map to a target table column name.Using this API extraction to a data table we can only read the data in the API.

  

Under this task type data is transmitted from URL to target destination by using GET method.

  

<b>Interpretation :  </b>

Approaching with Task type API allows you to interact with the tables and data inside the url and provides the exact data provided in the url to the client by using Get method.We involve Get Method in this Task type API which is used to request data from a specified resource and it cannot modify data as well.

<b>Navigation : </b> Navigate to Sql runner -> Create Job**
![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/JA1.png?raw=true)

**Select Task Type: API from drop-down list.**

Enter following details in create Job window:

-   **URL :**https://go.affiliatexe.com/api/admin/?fkp_username=ssssss&api_password=gPM1Onbv^O&command=report&fromdate=${key_start}&todate=${key_end}
    

-   **Method :** GET
    
-   **Key :** command
    
-   **Value :** commissions
    

  
  

-   **Block type:** Select **Date** from drop-down list.
    

-   **Block From & To:** enter start date and end date till where the data to fetched.
    

> **Block From** : 2020-11-08 YYYY|MM|DD **Block To** : 2020-11-09 YYYY|MM|DD

-   **Block Size:** Enter specific run time range.
    

> **Note: Block size:** 3 ( on selecting 1 runs daily, 2-runs once in two days and so on)

-   **Block Key From & To:** it works as reference name ( applicable in case of where conditions)
    

> **Block Key From:** Block Key: ${key_start} **Block Key To:** Block Key: ${key_end}

-   **Target Connection:**Select target database connection.

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/JA2.png?raw=true)

-   **Schema:** Select schema from drop down list.
    
-   **Table:** Select the target table from drop down list.
    
    -   **Insert/Update:** Insert or update target table.
        
    -   **Delete before insert:** Delete existing data before inserting target data.
        
    -   **Truncate Table before insert:** delete entire table before inserting target data.
        
- **Delete Reference :** Deletes previously existing records for blocks and reloads fresh data.
    
-   **Update Reference Fields :** it is a primary key based on given combination, data over writes the existing data.
    

-   **Field Mapping:** enable field mapping for source and target data.
    
-   Click on **Save** button to save the job.

<b>NOTE : </b> In Source database either PostgreSQL or Vertica the destination database should be Vertica only then

  

1. In Source Query need to add the ORDER BY with Primay key or Uniquer key columns (**original column name s not column alias**)

  
  

2. Need not specify the keywords like limit , offset , ; (semi -column) in source query and delete reference query

<!--stackedit_data:
eyJoaXN0b3J5IjpbNDM3ODc2MTQsLTEwNTM4MDU1MDMsLTU0OT
MzNTY0NSwtMTQwMTI5NzY2NF19
-->