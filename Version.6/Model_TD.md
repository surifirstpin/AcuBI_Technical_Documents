<center><h2>MODEL</h2></center>

This section introduces the steps to create a new project and accordingly generates a basic model from the database.
A model is a customized gateway into the database for accessing data as per business logic. AcuBi provides an IDE, which allows mappings between views (database tables) and apply several filters on the data as per business requirement. It is designed in such a way that it provides a spontaneous data analysis to specific business users.

**A model can be defined in 3 steps :**

-   Creating a Project with required database and respective tables.

-   Customize the Model using IDE as per the business requirement.

-   Organize the fields in Views with required manipulation.

## Creating a Project 

> **Navigation: Model → Projects → New Project**

### Step 1

**1.**  Click **New Project** button, to create a new project in a model.

![
](https://raw.githubusercontent.com/sv18042016/fp1/00615483357376318b721b9cf15a41579b9461ea/images/New_version5/TD_Model_image1.png)
**Image 1**

**Enter the following details;**

-   **Project Name:**  Enter the project name.
### Step 2    
-   **Connection:**  Choose the database connection from the drop-down list provided.

![
](https://raw.githubusercontent.com/sv18042016/fp1/67d93f76cb8e582b7157b1f8e696925b97fa4abd/images/New_version5/TD_Model_image2.png)
**Image 2**

###  Step 3
- **Database:** Choose the database for configuration. All the selected databases are visible under **Selected Databases** section.

![
](https://raw.githubusercontent.com/sv18042016/fp1/94a885c012491ba11e96367e359fc5a65526085e/images/New_version5/TD_Model_image3.png)
**Image 3**

### Step 4
- **Tables** Select the required tables from which data should be retrieved. Select the desired table fields from table section, All the selected tables are visible under **Selected Tables** section.

**2.** **Auto Build Joins (check box)** On selecting auto build checkbox,  it will adopt all the defined mappings or relations between different tables of a database and displays it in model. Else only tables with no mappings will be adopted as views in model.

![
](https://raw.githubusercontent.com/sv18042016/fp1/a7917cd2c9ad40f7abbfe85519a69bc3e9a8af45/images/New_version5/TD_Model_image4.png)
**Image 4**

### Step 5
-   **Privacy** you can save the project in any one of the following privacy option.
    -   **Private:**  report saved in private section are accessed by the existing user only.
    -   **Public:**  report is saved in public section are accessed by all the users.
   
    -   **Share:**  report saved under share section are accessed by specific set of users.
    
![
](https://raw.githubusercontent.com/sv18042016/fp1/ffa4998a87ebeece5d3fde4f2930b83243e9b4a8/images/New_version5/TD_Model_image5.png)
**Image 5**

**3.** Once all the entries are made, click on  **Save Project**  to save the project created.

> **Note:** All the saved projects are visible on left hand side under projects.

## Edit Project

- Click on Projects, select the desired project and hit the **Edit** button.

![
](https://raw.githubusercontent.com/sv18042016/fp1/e535debfb80662d425803114d0399ad21e615cda/images/New_version5/TD_Model_image6.png)
**Image 6**
- After making necessary changes hit the **Update** button to save the changes made.

- To cancel the changes made to a project hit **Cancel** button.

## Delete Project

To delete the project created hit the **Delete** icon, on far right of the project list.

![
](https://raw.githubusercontent.com/sv18042016/fp1/66530cb4c6a170b9703c654fdad1927190ba7a60/images/New_version5/TD_Model_image7.png)
**Image 7**

## Model and Customization

After saving a project, AcuBi will display the views and relevant information of the project as a **Model**, which can be further customized as per the business requirement. 
Once the project is saved, model screen is triggered.(Refer Image 8)
Depending on the table joins applied the code is retrieved in JSON format. To refresh the data, hit the refresh icon of model, project and tables.

**4.**  To undo the changes done click **Undo**.

**5.**  To redo the changes click  **Redo**.

**6.** To format the code, for a proper alignment, click **Format Code**.

![
](https://raw.githubusercontent.com/sv18042016/fp1/4822775225f357a86fd13bbd40a05c88bd0fca0a/images/New_version5/TD_Model_image8.png)
**Image 8**

**7.**  To hide and unhide model and views list click on **Angle double left** and **Angle double right** Icon.

**8.** To save the model click on **Save** button.

![
](https://raw.githubusercontent.com/sv18042016/fp1/277037f93bc45d7c04c5c27d596cc7e7e3adf0d5/images/New_version5/TD_Model_image9.png)
**Image 9**

**Customization for a model can be carried out in following ways :**

-  Add a new mapping or relations among the views based on a specific condition.

- Edit the join criteria between views.

-  Define filters on the data with different mapped views.


**The list of keywords used in Model are:**

|  **Serial No.** | **Keyword** | **Description** |
|  ------ | ------| ------ |
|  1 | **For Model** |  |
|   | project | displays the project name |
|   | info | allows to describe the project with meaning full information |
|   | connections | displays the connection name with the selected project |
|   | explore | displays the views (the tables selected in the project) with the selected characteristics |
|  2 | **For View** |  |
|   | name | name of the table used in database |
|   | label | allows you to customize the display name of the view in AcuBi|
|   | filters | the list of filters to be applied on the data from the view and respective mapped views defined in the 'joins"section |
|   | joins | specifies the list of associated views which are mapped with the current view & mention the mapping criteria |
|  2A | **Filter characteristics** | Filters can be date-based, string-based, value-based & user-based |
|   | name | name of the filter |
|   | Filter_sql | the query phrase which acts as a filter, eg: col name = “Employee Name’ |
|   | Apply | to specify the applicability |
|   | Position | describes the priority of the filter phrases to be assigned as 'before" or 'after" |
| |Bindkey|it is a string applied to a query in order to reduce the execution time of a custom query|
| |filterViewName| Name of the custom view in which the bindkey is used|
| |filterKey_mapping|The column mapping for a field against which the bindkey is used|
|  2B | **Joins characteristics** |  |
|   | join | derive the relationship between 2 views based on the condition. |
|   | join_type | derives type of join condition to be applied (Left,Right,inner join) |
|   | join_on | defines the relationship between views by associated fields. |

**2.A Filters in Model :**

To filter data from a view and the respective mapping views, the filter criteria can be defined in “filters” section.

```
{
"name": "View_Name",
"label": "View_Name",
"filters": [{
"name": "filter_name",                                 * filter name *
"filter_sql": Filter Expression ",                     * expression or condition to be applied*
"apply": "all",
"position": "before"                                   * position of filter *
           }],
"joins":[]
}

```

**Filter can be derived with two specific attributes such as;**

**I.**  **Filter_Sql :**  the filter expression or condition. Filter expression can be date-based, string-based, number-based and even login-based.

-  **Date-Based:** standard filters which are applicable on dates.
```
 ROOT.Orders.OrderDate < TRUNC(SYSDATE)  
```
-  **String-Based:** standard filters which are applicable on strings.
```
 ROOT.Orders.PaymentMode IN (‘Cash’,’PayTM’)
 ```
-  **Number-Based:**  standard filters which are applicable on numbers.
```
ROOT.BI_Orders.Amount IS NOT NULL
```
-   **User-based:** AcuBi allows to filter the data based on login user-specification. Using global parameters facility, data for the same combination of columns can be controlled for different users i.e for a particular user login, the data retrievable in analyze section will be constrained with a list of pre-defined values.
```
 " DB.TABLE.COLUMN IN (#{GlobalParam.Ref_field,#userid#,gp_username_field})" 
```
-   **GlobalParam:**  the name of the global parameter which contains the user based list of values.
-   **Ref_Field**  the column name in global parameter which contains the filter values.
-   **Gp_Username_Field**  the column name in global parameter which contains the usernames.
```
" ROOT.Orders.StationCode IN (#{ModelParams.StationCode,#userid#,Username})"
```
**II.**  **Position**  Assigning filter “before” or “after" the data.
-   **Before**  the filter will be applied first to the data, before any alternate filters on data are applied in report section.
-   **After**  the filter will be applied to the data after applying filters in report section.

**2.B. Join Characteristics**

**Join attributes are defined as follows :**

-   **Join** the view name to be joined with the primary view.
-   **Join_type**  the method of joining two views. Either left or right is similar to “**Join**” functionality.
-   **Join_on**  the specific criteria of joining the views with a relation among relevant fields.

```
{
"name": "View_1",                                       * Primary View *
"label": "View_1",
"filters":[],
"joins":
[ 
{
"join": "View_2",                                       * Secondary View *
"join_type": "left",                                    * Type of Join *
"join_on": "${View_1.Field} = ${View_2.Field}"          * Join criteria*
} 
]
}
```
## Views and Fields

Views are independent tables chosen while creating a project. All the columns in the table are called fields of view and will be adopted with relevant features.

**AcuBi allows various actions to performed in views as follows:**

-  Creating a new field (User Defined Fields).
-  Defining the output in a new field as resultant of arithmetical or logical operations among the database fields of the self view or from mapped views.
-  Assigning currency & number format for measure fields.
-  Extracting different date formats from the date field permissible formats like hour, day, week, month, quarter, year, date, week_day, date_month, date_quarter, date_hour, year_week.
-  You can create new custom views.
-  Assigning drill down fields for a field.
-  Defining values for different map co-ordinates.

The Associated keywords with the views are flowing :

|  **S.No** | **Name** | **Identifier of a custom field** |
|  :------ | :------: | :------: |
|  1 | label | allows to customize the display name of the view in AcuBi |
|  2 | data_type | the outcome of the field from database it can be string, date or number |
|  3 | type | either of the two values dimension or measure, string and date belongs to dimension and number belongs to measure |
|  4 | time_frame | feature that extract different formats from the date field, for instance: hour,day,week, month quarter; year, date. week_day,date_ month date_quarter date_hour, year_week |
|  5 | lookup | a set of filter values for a specific field ether from database using a query or from a defined item list |
|  6 | operator | the option to select single or multiple filters from the assigned lookup |
|  7 | sql | the query phase which retrieves the data from database Ex: $ {TABLE }. username |
|  8 | summary | the option to aggregate a measure field.For instance Supports sum avg, count, min, max. |
|  9 | drill_down_fields | the option to define the drill fields for the current field |
|  10 | show_drill_down_measures | it carry forward the current state of measures to further drill level. It can applied using true or false condition |
|  11 | visualize | it controls the visibility of the field in Analyze section |
|  12 | number_format | to define a number format for the field. the list of valid formats are described as Amexure 1 |
|  13 | currency | it defines the currency for the field.For instance “$”, “€”, “£”, “₹”. |
|  14 | country_ref | option for enabling map view for different values with different geographical locations |
| 15 | always_filter | to directly define desired filters values in model itself. **for example** define "always_filter": "STATIONCODE IN ('Station_1','Station_2')"  it retrieves only station 1 and station 2 in analysis data section.|

**Among the above stated list, the following are the special attributes for user convenience :**

**I.**  **lookup and operator :**  Using “lookup” feature, AcuBi allows you to define a set of filter values for a field. The assignment can be made in the following two ways:
-   **Query**  an sql query returning a set of values can be written in **“lookup”** for a field. It will be useful if the filter values are large in number and becomes tedious to mention all of them as a list.
```
 “lookup” : “SELECT DISTINCT Name FROM ROOT.Employees”
```
-   **Items**  known set of values can be given with comma separation. It may be useful if the list is small and the items are known exactly to the user.

> **For Instance** :
 “lookup” : “Antonio, Bessanio, Portia”

-   **Operator**  Sometimes, data to be retrieved from multiple filter values. AcuBi provides an option associated with lookup which can be defined to select single or multiple filter values. For selecting more than one filter value, operator should be defined as **“multiple”** or else leave it empty.

```
operator:"",                        **Single operator**
```
```
operator:multiple.                  **Multiple operator**
```
**II.**  **Number_format & currency**  for reports convenience, a particular number format and currency can be assigned to a particular field so that whenever the report is created using this field, the number_format and currency will automatically displayed.

-   **Number_format**  There are various formats designed based on the common business usage.

**The permissible list are :**
> **For Instance:**
Consider Number = 12345679

|  S. No. | Number format | Example |
|  :------ | ------ | :------ |
|  1 | # | 12345679 |
|  2 | #.0 | 12345678.6 |
|  3 | #.00 | 12345678.57 |
|  4 | #.000 | 12345678.567 |
|  5 | #,##0 | 1.23.45,679 |
|  6 | #.##0.00 | 1.23.45,678.6 |
|  7 | #,##0.00 | 1.23.45,678.57 |
|  8 | #,##0.000 | 1.23.45.678.567 |
|  9 | ##,### | 12.345.679 |
|  10 | ###,###,0 | 12.345.678.6 |
|  11 | ###,###,0 | 12.345.678.57 |
|  12 | ###,###,000 | 12.345.678.567 |
|  13 | ###,###,0 | 12.345.678.6 |
|  14 | ###,###,00 | 12.345.678.57 |
|  15 | ###,###,000 | 12.345.678.567 |
|  16 | ### ### | 12 345 679 |
|  17 | #% | 12345679 |
|  18 | #,00% | 123456.786 |
|  19 | #,00% | 123456.7857 |
|  20 | #,000% | 123456.78567 |
|  21 | #K | 12345 678566999999k |
|  22 | #M | 12.345678567IM |

-   **Currency**  AcuBi supports following currency formats “$”, “€”, “£”, “₹”.

```
currency : currency_symbol
```
 **Example** : “currency” : “$”

**III.**  **Time_frame:** AcuBi provides an option to extract different components associated with time stamp for user convenience.

**Below are the formats adopted by default :**

|  **S No.** | **Component** | **Description** |
|  :------: | :------: | :------: |
|  1 | Hour | Extract hour component |
|  2 | Day | Extract day number in the month |
|  3 | Week | Extract week number in the year |
|  4 | Month | Extract month name |
|  5 | Quarter | Extract quarter number in the year |
|  6 | Year | Extract year component |
|  7 | Week_day | Extract the day component in the week |
|  8 | Date_month | Extract date in the respective Month component |
|  9 | Date_quarter | Extract year and respective Quarter component |
|  10 | Date_hour | Extract Date and respective Hour component |
|  11 | Year_week | Extract year and respective week component |
|  12  | Date     | Extracts respective date  |

## User Defined Fields (UDF)

AcuBi has an ability to create new fields in a view with all attributes that are applicable to a database field and with return value (“sql” section of the field) as any of the following options:

**1.**  As a resultant of arithmetical operations done on fields of the same view.
```
"sql": "(${TABLE}.Field1 arithmetical operation ${TABLE}.Field2)"
```

>**For Instance:** 
“sql”: “(${TABLE}.Amount + ${TABLE}.Discount)”

**2.**  As a resultant of arithmetical operations done on fields of a mapped view.

```
"sql": "(${TABLE}.Field1 arithmetical operation ${Mapped_View.Field})"
```

>**For Instance:** 
“sql”: “(${TABLE}.Amount) / ${Customers.Total_number})”

**3.**  As a resultant of logical operations ( like case statement ) done on fields of the same view.
```
 "sql": "(case when (condition) then Expression_1 else Expression_2 end) "
```

Where condition is an expression on the fields of self view and Expression_1, Expression_2 are expressions which include fields of self view.

> **For Instance:** 
 “sql”: “(CASE WHEN (${TABLE}.Name is not null) THEN ${TABLE}.Salary ELSE 0 END)”

**4.**  As a resultant of logical operations ( like case statement ) done on fields of a mapped view.

```
 "sql": "(case when (condition) then Expression_1 else Expression_2 end) "
```

Where condition is an expression defined on the fields of self view or mapped view and Expression_1, Expression_2 are expressions which include fields of self view or mapped view.

> **For Instance:** 
  “sql”: “(CASE WHEN (${[Customers.ID](http://customers.id/)} is not null) THEN ${TABLE}.Amount ELSE 0 END)”

**5.**  As a resultant of database function operated on fields.

```
   "sql": "(${TABLE}.Field * ${DB}.function_name(parameters)) "
```

> **Example**  “sql” : “(${TABLE}.Amount  KaTeX parse error: Expected 'EOF', got '​' at position 51: …te(DB.exchanger​̲ate({TABLE}.OrderDate,${TABLE}. CurrencyID))”

**6.**  As a resultant of string, date, number based sql functions on fields

```
  "sql" : "sql_function(${TABLE}.Field)"
```

> **For Instance:** 
Number → “sql” : “SUM($ {TABLE}.Amount)”,  
Date → “sql” : "TO_CHAR ( $ { TABLE}.OrderDate,‘Mon-YYYY’)"  
String → “sql” : “CONCAT('Date : ',${TABLE}.OrderDate)”

**7.**  As a resultant of single value returning sql query

```
   "sql" : "(select Expression from Database.Table)"
```

Where the expression contain the fields of self view and should result a single value.
```
 “sql”: "(select sum(x.Amount) from Orders)”
```
## Custom View

Custom fields are user defined fields for which we apply arithmetic  and logical operations that are supported by database. A view may join other views and there relationship are defined as part of data analysis section of model file.

### New Custom View

**1.** Click on **New Empty view** to create or derive a new custom view table.

![
](https://raw.githubusercontent.com/sv18042016/fp1/cf5946b2b83468c906303fc1b8480de242f0d17b/images/New_version5/TD_Model_image10.png)
**Image 10**

Once the view is created, label the database field and derive the custom table using a SQL query as a result a derived table is created.
``` 
{
"name": "CustomView_820",
	"label": "CustomView_820",
	"info": "Description",
	"type": "query",
	"sql": "(SELECT A.STATIONCODE SC,A.ORDERID ORID,A.WHENMADE ORTIME,B.NAME RECEPNAME, A.AMOUNT ORDVAL,A.QUANTITY QTY,A.WAYUSED ORDBY, A.PAYMENTMODE PM,C.NAME CUSTNAME,C.ADDRESS CUSTADDR FROM ROOT.ORDERS A INNER JOIN ROOT.EMPLOYEES B ON A.ORDERATTDID=B.EMPLOYEEID INNER JOIN ROOT.CUSTOMERS C ON A.CUSTOMERID=C.CUSTOMERID)",
	"database": "ROOT",
	"connection": "Oracle_Build",
"fields": [
		{
			"name": "SC",
			"label": "STATION CODE",
			"data_type": "string",
			"type": "dimension",
			"lookup": "",
			"operators": "",
			"sql": "\"CustomView_791\".SC",
			"summary": "",
			"visualise": "true",
			"country_ref": {
				"Station_1": "IND",
				"Station_2": "AUS"
			               }
		},
		{
			"name": "ORID",
			"label": "ORDERSCOUNT",
			"data_type": "number",
			"type": "measure",
			"lookup": "",
			"operators": "",
			"sql": "COUNT(DISTINCT \"CustomView_820\".ORID)",
			"summary": "",
			"visualise": "true"
		},
		]
}
```
- **Name** name identifier of custom table derived.
- **label** label the custom table the way it should appear in model section. 
- **Info** provides description for custom table.
- **Type** datatype used for deriving a custom table.
- **Database** table is used to retrieve the data fields.
- **Connection** establish the database connection for deriving new fields.
## Save View

Click **Save** to Save the View in database.

![
](https://raw.githubusercontent.com/sv18042016/fp1/55cfae57f76a2b3fd0dc9dacb855113be7260f7d/images/New_version5/TD_Model_image11.png)
**Image 11**
##  Arithmetical operations in Custom Fields
```
{
			"name": "SC_SUBSTR",
			"label": "SC_SUBSTR",
			"data_type": "string",
			"type": "dimension",
			"lookup": "",
			"operators": "",
			"sql": "SUBSTR(${TABLE}.STATIONCODE,1,4)",
			"summary": "",
			"visualise": "true"
},
		{
			"name": "SC_SUBSTR1",
			"label": "SC_SUBSTR1",
			"data_type": "string",
			"type": "dimension",
			"lookup": "",
			"operators": "",
			"sql": "SUBSTR(${TABLE}.STATIONCODE,5,7)",
			"summary": "",
			"visualise": "true"
		},
		{
			"name": "SC_CONCAT",
			"label": "SC_CONCAT",
			"data_type": "string",
			"type": "dimension",
			"lookup": "",
			"operators": "",
			"sql": "CONCAT(SUBSTR(${TABLE}.STATIONCODE,1,4),SUBSTR(${TABLE}.STATIONCODE,5,7))",
			"summary": "",
			"visualise": "true"
		},
```	

- **Name** identifier for the field in custom table.
- **label**  the way derived field should display in custom table.
- **Data_type** define supporting parameters and string is used as  default parameter while deriving the fields for custom table.
   - **String** for measures that contain letters or special characters.
  - **Date** measures that contain dates.
  - **Time_frame** is a derived list of formats from time stamps for instance the following are the available formats hour, day, week,month,quarter, year,date,week_day, date_month, date_quarter, date_hour, year_week.
  - **Number** for the measure that contain number.
  - **Int** for the measure that contains integers.
  - **Type** can be used as part of dimension or measure.

## Lookups

- **lookup** retrieve list of values for a specific field either from database using a query or from an item list (it is listed in the filter section during visualization).
- **Operator** is used to retrieve single or multiple values in the filter section while using lookup.
 - **SQL** parameter is used to define a valid SQL expression that results in a field value.
 - **Summary** is used to retrieve the aggregate field values of the measures using the following options,
   - Sum 
   - Count
   - Average 
   - Maximum
   - Minimum

## Drill-Down 

Drill-down is used for exploring the data further with respect to a field value. AcuBi has an ability to define drill option for a field with a set of derivable fields and when clicked on a particular value of an assigned field, the individual records that make up that cell will be displayed by limiting the query with the clicked value.

## Show Drill-Down Measures

Sometimes, it may be necessary to bring the current stage measure fields to the next drill stage along with the drill fields.

AcuBi provides an additional attribute to drill down as  **Show drill down measures**  which can be defined as  **TRUE or FALSE**. If mentioned TRUE, then system will carry forward the measures of the current stage to the immediate drill level.

```
"drill_down_fields": "Field1,Field2,...FieldN."
```

“show_drill_down_measures”: “true / false”  
```
 {  
 “name”: “StateName”,  
 “label”: “StateName”,  
 “data_type”: “string”,  
 “type”: “dimension”,  
 “lookup”: “”,  
 “operators”: “”,  
 “sql”: “${TABLE}.StateName”,  
 “summary”: “”,  
 “drill_down_fields”: “CityName,No_of_Employees”,  
 “show_drill_down_measures”: “true”,  
 “visualise”: “true”  
 }
```
In the above example, Drill down option is defined over field “**State Name**” with two fields of self view City Name, No_of_Employees. On Clicking on any of “State Name”, then filter will be applied on that value and relevant values of fields **“City Name”** and **“No_of_Employees”** will be displayed.

As  **Show drill down measures**  is set  **TRUE**, the associated measures (if exists) of the field “State Name” will also be brought to the next stage along with drill fields City Name and No_of_Employees.



# Maps

Maps enables users to visualize the geographic data on reactive and interactive maps. To carry out maps  in AcuBi,Your query should include at least one dimension based on geographic data. On including measure in your query it will display the information about the location selected.

To carryout maps under visualization you need to derive the data fields in Model Section initially.

 **For Model, Views and for a specific field the map co-ordinates  may be assigned as follows :**
```
{
"name": "Field",
"label": "Field",
"data_type": "string",
"type": "dimension",
"lookup": "",
"operators": "",
"sql": "${TABLE}.DB\_Column\_Name",
"summary": "",
"visualise": "true",
"country_ref": {
"Field_Value_1": "IND",
"Field_Value_2": "AUS",
"Field_Value_N": "Country",   
               }
}
```
```
{
			"name": "SC",
			"label": "STATION CODE",
			"data_type": "string",
			"type": "dimension",
			"lookup": "",
			"operators": "",
			"sql": "${TABLE}.SC",
			"summary": "",
			"visualise": "true",
			"country_ref": {
				"Station_1": "IND",
				"Station_2": "AUS"
			               }
}
```

**The allowed list of country codes are :**


|  Country Name | Code |  | Country Name | Code |  | Country Name | Code |  | Country Name | Code |  | Country Name | Code |
|  ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
|  Aruba | ABW |  | Colombia | COL |  | Croatia | HRV |  | Mozambique | MOZ |  | El Salvador | SLV |
|  Afghanistan | AFG |  | Comoros | COM |  | Haiti | HTI |  | Mauritania | MRT |  | San Marino | SMR |
|  Angola | AGO |  | Cape Verde | CPV |  | Hungary | HUN |  | Montserrat | MSR |  | Somalia | SOM |
|  Anguilla | AIA |  | Costa Rica | CRI |  | Indonesia | IDN |  | Martinique | MTQ |  | Saint Pierre and Miquelon | SPM |
|  Aland Islands | ALA |  | Cuba | CUB |  | Isle of Man | IMN |  | Mauritius | MUS |  | Serbia | SRB |
|  Albania | ALB |  | Christmas Island | CXR |  | India | IND |  | Malawi | MWI |  | South Sudan | SSD |
|  Andorra | AND |  | Cayman Islands | CYM |  | British Indian Ocean Territory | IOT |  | Malaysia | MYS |  | Sao Tome and Principe | STP |
|  Netherlands Antilles | ANT |  | Cyprus | CYP |  | Ireland | IRL |  | Mayotte | MYT |  | Suriname | SUR |
|  United Arab Emirates | ARE |  | Czech Republic | CZE |  | Iran, Islamic Republic of | IRN |  | Namibia | NAM |  | Slovakia | SVK |
|  Argentina | ARG |  | Germany | DEU |  | Iraq | IRQ |  | New Caledonia | NCL |  | Slovenia | SVN |
|  Armenia | ARM |  | Djibouti | DJI |  | Iceland | ISL |  | Niger | NER |  | Sweden | SWE |
|  American Samoa | ASM |  | Dominica | DMA |  | Israel | ISR |  | Norfolk Island | NFK |  | Swaziland | SWZ |
|  Antarctica | ATA |  | Denmark | DNK |  | Italy | ITA |  | Nigeria | NGA |  | Seychelles | SYC |
|  French Southern Territories | ATF |  | Dominican Republic | DOM |  | Jamaica | JAM |  | Nicaragua | NIC |  | Syrian Arab Republic (Syria) | SYR |
|  Antigua and Barbuda | ATG |  | Algeria | DZA |  | Jersey | JEY |  | Niue | NIU |  | Turks and Caicos Islands | TCA |
|  Australia | AUS |  | Ecuador | ECU |  | Jordan | JOR |  | Netherlands | NLD |  | Chad | TCD |
|  Austria | AUT |  | Egypt | EGY |  | Japan | JPN |  | Norway | NOR |  | Togo | TGO |
|  Azerbaijan | AZE |  | Eritrea | ERI |  | Kazakhstan | KAZ |  | Nepal | NPL |  | Thailand | THA |
|  Burundi | BDI |  | Western Sahara | ESH |  | Kenya | KEN |  | Nauru | NRU |  | Tajikistan | TJK |
|  Belgium | BEL |  | Spain | ESP |  | Kyrgyzstan | KGZ |  | New Zealand | NZL |  | Tokelau | TKL |
|  Benin | BEN |  | Estonia | EST |  | Cambodia | KHM |  | Oman | OMN |  | Turkmenistan | TKM |
|  Burkina Faso | BFA |  | Ethiopia | ETH |  | Kuwait | KWT |  | Pakistan | PAK |  | Timor-Leste | TLS |
|  Bangladesh | BGD |  | Finland | FIN |  | Lao PDR | LAO |  | Panama | PAN |  | Tonga | TON |
|  Bulgaria | BGR |  | Fiji | FJI |  | Lebanon | LBN |  | Pitcairn | PCN |  | Trinidad and Tobago | TTO |
|  Bahrain | BHR |  | Falkland Islands (Malvinas) | FLK |  | Liberia | LBR |  | Peru | PER |  | Tunisia | TUN |
|  Bahamas | BHS |  | France | FRA |  | Libya | LBY |  | Philippines | PHL |  | Turkey | TUR |
|  Bosnia and Herzegovina | BIH |  | Faroe Islands | FRO |  | Saint Lucia | LCA |  | Palau | PLW |  | Tuvalu | TUV |
|  Saint-Barthélemy | BLM |  | Micronesia, Federated States of | FSM |  | Liechtenstein | LIE |  | Papua New Guinea | PNG |  | Taiwan, Republic of China | TWN |
|  Belarus | BLR |  | Gabon | GAB |  | Sri Lanka | LKA |  | Poland | POL |  | Tanzania, United Republic of | TZA |
|  Belize | BLZ |  | United Kingdom | GBR |  | Lesotho | LSO |  | Puerto Rico | PRI |  | Uganda | UGA |
|  Bermuda | BMU |  | Georgia | GEO |  | Lithuania | LTU |  | Korea (North) | PRK |  | Ukraine | UKR |
|  Bolivia | BOL |  | Guernsey | GGY |  | Luxembourg | LUX |  | Portugal | PRT |  | US Minor Outlying Islands | UMI |
|  Brazil | BRA |  | Ghana | GHA |  | Latvia | LVA |  | Paraguay | PRY |  | Uruguay | URY |
|  Barbados | BRB |  | Gibraltar | GIB |  | Macao, SAR China | MAC |  | Palestinian Territory | PSE |  | United States of America | USA |
|  Brunei Darussalam | BRN |  | Guinea | GIN |  | Saint-Martin (French part) | MAF |  | French Polynesia | PYF |  | Uzbekistan | UZB |
|  Bhutan | BTN |  | Guadeloupe | GLP |  | Morocco | MAR |  | Qatar | QAT |  | Holy See (Vatican City State) | VAT |
|  Bouvet Island | BVT |  | Gambia | GMB |  | Monaco | MCO |  | Réunion | REU |  | Saint Vincent and Grenadines | VCT |
|  Botswana | BWA |  | Guinea-Bissau | GNB |  | Moldova | MDA |  | Romania | ROU |  | Venezuela (Bolivarian Republic) | VEN |
|  Central African Republic | CAF |  | Equatorial Guinea | GNQ |  | Madagascar | MDG |  | Russian Federation | RUS |  | British Virgin Islands | VGB |
|  Canada | CAN |  | Greece | GRC |  | Maldives | MDV |  | Rwanda | RWA |  | Virgin Islands, US | VIR |
|  Cocos (Keeling) Islands | CCK |  | Grenada | GRD |  | Mexico | MEX |  | Saudi Arabia | SAU |  | VietNam | VNM |
|  Switzerland | CHE |  | Greenland | GRL |  | Marshall Islands | MHL |  | Sudan | SDN |  | Vanuatu | VUT |
|  Chile | CHL |  | Guatemala | GTM |  | Macedonia, Republic of | MKD |  | Senegal | SEN |  | Wallis and Futuna Islands | WLF |
|  China | CHN |  | French Guiana | GUF |  | Mali | MLI |  | Singapore | SGP |  | Samoa | WSM |
|  Côte d'Ivoire | CIV |  | Guam | GUM |  | Malta | MLT |  | South Georgia and the South Sandwich Islands | SGS |  | Yemen | YEM |
|  Cameroon | CMR |  | Guyana | GUY |  | Myanmar | MMR |  | Saint Helena | SHN |  | South Africa | ZAF |
|  Congo, (Kinshasa) | COD |  | Hong Kong, SAR China | HKG |  | Montenegro | MNE |  | Svalbard and Jan Mayen Islands | SJM |  | Zambia | ZMB |
|  Congo (Brazzaville) | COG |  | Heard and Mcdonald Islands | HMD |  | Mongolia | MNG |  | Solomon Islands | SLB |  | Zimbabwe | ZWE |
|  Cook Islands | COK |  | Honduras | HND |  | Northern Mariana Islands | MNP |  | Sierra Leone | SLE |  

## Existing Projects and Views

To view and access the existing projects and views, click on 
move the cursor to projects on top left of the screen then click the drop-down to display the list of projects created. Simultaneously on selecting the projects it displays the list of views that fall under that particular project created.

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0NDg2NTIwMjAsLTYxMzk2ODc3NSwxMT
YyMDQ0NzU5LC0xNjA3ODMyNjY1LDIxMjU4MTY1Myw1Nzg0ODI0
NywyMDY5MDQ3NzM1XX0=
-->