
<center><h1>MODEL</h1></center>

This section introduces steps to create a new project and accordingly generates a basic model from the database.
A model is a customized gateway into the database for accessing data as per business logic. AcuBi provides an IDE, which allows mappings between views (database tables) and apply several filters on the data as per business requirement. It is designed in such a way that it provides a spontaneous data analysis to specific business users.

<b><i><u>A model can be defined in 3 steps :</u></i></b>

-   Creating a Project with required Database and respective Tables.

-  Customize the Model using IDE as per the business requirement.

-  Organize the fields in Views with required manipulation.

## Creating a Project 

> <b>Navigation: Model → Projects → New Project</b>

### Step 1:

<b>1.</b>  Click <b>New Project</b> button, to create a new project in a model.

![
](https://raw.githubusercontent.com/sv18042016/fp1/00615483357376318b721b9cf15a41579b9461ea/images/New_version5/TD_Model_image1.png)
<b><Font color = " black">Image 1</font></b>

<b><i><u>Enter the following details; </u></i></b>

<b>Project Name:</b>  Enter the project name.

### Step 2:    

<b>Connection :</b>  Choose the database connection from the drop-down list provided.

![
](https://raw.githubusercontent.com/sv18042016/fp1/67d93f76cb8e582b7157b1f8e696925b97fa4abd/images/New_version5/TD_Model_image2.png)
 <b><Font color = " black">Image 2</font></b>
 
###  Step 3:
<b>Database:</b> Choose the database for configuration. All the selected databases are visible under <b>Selected Databases Section.</b> 

![
](https://raw.githubusercontent.com/sv18042016/fp1/94a885c012491ba11e96367e359fc5a65526085e/images/New_version5/TD_Model_image3.png)
 <b><Font color = " black">Image 3</font></b>
 
### Step 4:

 <b>Tables:</b> Select the required tables from which data should be retrieved. Select the desired table fields from table section, All the selected tables are visible under <b>Selected Tables</b> section.

<b>2.</b> <b>Auto Build Joins: (check box)</b> On selecting auto build checkbox,  it will adopt all the defined mappings or relations between different tables of a database and displays it in model. Else only tables with no mappings will be adopted as views in model.


<b> Note: </b>  Auto build joins are added only while creating a project.

![
](https://raw.githubusercontent.com/sv18042016/fp1/a7917cd2c9ad40f7abbfe85519a69bc3e9a8af45/images/New_version5/TD_Model_image4.png)
 <b><Font color = " black">Image 4</font></b>
 
### Step 5:

<b>Privacy:</b> you can save project in any one of the following privacy option.
   -   <b>Private:</b>  report saved in private section are accessed by the existing user only.
   
   -   <b>Public:</b>  report is saved in public section are accessed by all the users.
   
   -   <b>Share:</b>  report saved under share section are accessed by specific set of users.
    
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/ffa4998a87ebeece5d3fde4f2930b83243e9b4a8/images/New_version5/TD_Model_image5.png)

 <b><Font color = " black">Image 5</font></b>
 

<b>3.</b> Once all the entries are made, click on  <b>
Save Project</b>  to save the project created.

> <b>Note:</b> All the saved projects are visible under projects list.

## Edit Project

Click Projects, select the desired project and hit the <b>Edit</b> button.

![
](https://raw.githubusercontent.com/sv18042016/fp1/e535debfb80662d425803114d0399ad21e615cda/images/New_version5/TD_Model_image6.png)
 <b><Font color = " black">Image 6</font></b>
 
- After making necessary changes hit the <b>Update</b> button to save the changes made.

- To cancel the changes made to a project hit <b>Cancel</b> button.

## Delete Project

To delete a project click  <b>Delete </b> icon available on far right of the project name under projects list.

![
](https://raw.githubusercontent.com/sv18042016/fp1/66530cb4c6a170b9703c654fdad1927190ba7a60/images/New_version5/TD_Model_image7.png)
 <b><Font color = "black">Image 7</font></b>

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/df368df5684e0a888b88d3673406f7525e1c4275/images/New_version5/td_model_image19.png)

## Existing Projects and Views

To view and access existing <b>Projects and Views,</b> hit projects button on top right of the screen, it will display list of projects created.  on selecting a project using a drop-down, it will display the list of views that fall under projects.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/a7598abcf90c0b79199f02f9eaae652de00108e0/images/New_version5/TD_Model_image20.png)
<b><Font color = " black">Image 8</font></b>
> Note : Tables added to a project are visible as views on initial screen.

Below image displays list of projects created. Select project name under the list to view the project.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/685d353bb1f288ee590b8a6ac3a2994c7ef6eb23/images/New_version5/TD_Model_image12.png)
<b><Font color = " black">Image 9</font></b>

## Model and Customization

After saving a project, AcuBi will display the views and relevant information of the project as a <b>Model</b>, which can be further customized as per the business requirement. Once the project is saved, model screen is triggered.
Depending on the table joins applied the code is retrieved in <b>JSON</b> format. To refresh the data, hit the refresh icon of model, project and tables.

<b>4.</b>  To undo the changes done click <b>Undo</b>.

<b>5.</b>  To redo the changes click  <b>Redo.</b>

<b>6.</b> To format the code, for a proper alignment, click <b>Format Code</b>.

![
](https://raw.githubusercontent.com/sv18042016/fp1/4822775225f357a86fd13bbd40a05c88bd0fca0a/images/New_version5/TD_Model_image8.png)
 <b><Font color = " black">Image 9</font></b>

<b>7.</b>  To hide and un-hide model and views list click on <b>Angle double left</b> and <b>Angle double right</b> Icon.


## Save

<b>8.</b> To save the model click on <b>Save</b> button.

![
](https://raw.githubusercontent.com/sv18042016/fp1/277037f93bc45d7c04c5c27d596cc7e7e3adf0d5/images/New_version5/TD_Model_image9.png)
 <b><Font color = " black">Image 10</font></b>

<b><i><u>Customization for a model can be carried out in following ways :</u></i></b>

-  Add a new mapping or relations among the views based on a specific condition.

- Edit the join criteria between views.

-  Define filters on the data with different mapped views.


<b><i><u>The list of keywords used in Model are:</u></i></b>

|  <b>Serial No.</b> | <b>Keyword</b> | <b>Description</b> |
|  ------ | ------| ------ |
|  1 | <b>For Model</b> |  |
|   | project | displays the project name |
|   | info | allows to describe the project with meaning full information |
|   | connections | displays the connection name with the selected project |
|   | explore | displays the views (the tables selected in the project) with the selected characteristics |
|  2 | <b>For View</b> |  |
|   | name | name of the table used in database |
|   | label | allows you to customize the display name of the view in AcuBi|
|   | filters | the list of filters to be applied on the data from the view and respective mapped views defined in the 'joins"section |
|   | joins | specifies the list of associated views which are mapped with the current view & mention the mapping criteria |
|  2A | <b>Filter characteristics</b> | Filters can be date-based, string-based, value-based & user-based |
|   | name | name of the filter |
|   | Filter_sql | the query phrase which acts as a filter, eg: col name = “Employee Name’ |
|   | Apply | to specify the applicability |
|   | Position | describes the priority of the filter phrases to be assigned as 'before" or 'after" |
| |Bindkey|it is a string applied to a query in order to reduce the execution time of a custom query|
| |filterViewName| Name of the custom view in which the bindkey is used|
| |filterKey_mapping|The column mapping for a field against which the bindkey is used|
|  2B | <b>Joins characteristics</b> |  |
|   | join | derive the relationship between 2 views based on the condition. |
|   | join_type | derives type of join condition to be applied (Left,Right,Inner Join) |
|   | join_on | defines the relationship between views by associated fields. |

<b>2.A Filters in Model :</b>

To filter data from a view and the respective mapping views, the filter criteria can be defined in “filters” section.


```
{
"name": "View_Name",
"label": "View_Name",
"filters": [{
"name": "filter_name",                                 *filter name*
"filter_sql": Filter Expression ",                     * expression or condition to be applied*
"apply": "all",
"position": "before"                                   *position of filter*
           }],
"joins":[]
}

```

<b><i><u>Filter can be derived with two specific attributes such as;</u></i></b>

<b>I.</b>  <b>Filter_Sql :</b>  the filter expression or condition. Filter expression can be date-based, string-based, number-based and even login-based.

<b>Date-Based:</b> standard filters which are applicable on dates.
```
 ROOT.Orders.OrderDate < TRUNC(SYSDATE)  
```
<b>String-Based:</b> standard filters which are applicable on strings.
```
 ROOT.Orders.PaymentMode IN (‘Cash’,’PayTM’)
 ```
<b>Number-Based:</b>  standard filters which are applicable on numbers.
```
ROOT.BI_Orders.Amount IS NOT NULL
```
 <b>User-based:</b> AcuBi allows to filter the data based on login user-specification. Using global parameters facility, data for the same combination of columns can be controlled for different users i.e for a particular user login, the data retrievable in analyze section will be constrained with a list of pre-defined values.
```
 " DB.TABLE.COLUMN IN (#{GlobalParam.Ref_field,#userid#,gp_username_field})" 
```
 <b>GlobalParam:</b> the name of the global parameter which contains the user based list of values.

<b>Ref_Field</b>  the column name in global parameter which contains the filter values.

<b>Gp_Username_Field</b>  the column name in global parameter which contains the usernames.
```
" ROOT.Orders.StationCode IN (#{ModelParams.StationCode,#userid#,Username})"
```
<b>II.</b> <b>Position</b>  Assigning filter “before” or “after" the data.
-   <b>Before</b>  the filter will be applied first to the data, before any alternate filters on data are applied in report section.

-   <b>After</b>  the filter will be applied to the data after applying filters in report section.

<b>2.B. Join Characteristics</b>

<b>Join attributes are defined as follows :</b>

-   <b>Join</b> the view name to be joined with the primary view.

-   <b>Join_type</b>  the method of joining two views. Either left or right is similar to <b>Join</b> functionality.

-   <b>Join_on</b>  the specific criteria of joining the views with a relation among relevant fields.

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

<b><i><u>AcuBi allows various actions to performed in views as follows:</u></i></b>

-  Creating a new field (User Defined Fields).

-  Defining the output in a new field as resultant of arithmetical or logical operations among the database fields of the self view or from mapped views.

-  Assigning currency & number format for measure fields.

-  Extracting different date formats from the date field permissible formats like hour, day, week, month, quarter, year, date, week_day, date_month, date_quarter, date_hour, year_week.

-  You can create new custom views.

-  Assigning drill down fields for a field.

-  Defining values for different map co-ordinates.

<b><i><u>The Associated keywords with the views are flowing :</u></i></b>

|  <b>S.No | Name | Identifier of a custom field </b> |
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
| 15 | always_filter | to directly define desired filters values in model itself. <b>for example</b> define "always_filter": "STATIONCODE IN ('Station_1','Station_2')"  it retrieves only station 1 and station 2 in analysis data section.|
| 16 | Time_frame_grouping | If it is enabled as true.Grouping under dashboard filters is enabled.(applicable only for date fields)|

<b><i><u>Among the above stated list, the following are the special attributes for user convenience :</u></i></b>

<b>I.  lookup and operator :</b>  Using “lookup” feature, AcuBi allows you to define a set of filter values for a field. The assignment can be made in the following two ways:
-   <b>Query</b>  an sql query returning a set of values can be written in <b>“lookup”</b> for a field. It will be useful if the filter values are large in number and becomes tedious to mention all of them as a list.
```
 “lookup” : “SELECT DISTINCT Name FROM ROOT.Employees”
```
-   <b>Items</b>  known set of values can be given with comma separation. It may be useful if the list is small and the items are known exactly to the user.

> <b>For Instance</b> :
 “lookup” : “Antonio, Bessanio, Portia”

-   <b>Operator</b>  Sometimes, data to be retrieved from multiple filter values. AcuBi provides an option associated with lookup which can be defined to select single or multiple filter values. For selecting more than one filter value, operator should be defined as <b>“multiple”</b> or else leave it empty.

```
operator:"",                        **Single operator**
```
```
operator:multiple.                  **Multiple operator**
```
<b>II. Number_format & currency</b>  for reports convenience, a particular number format and currency can be assigned to a particular field so that whenever the report is created using this field, the number_format and currency will automatically displayed.

-   <b>Number_format</b> There are various formats designed based on the common business usage.

<b><i>The permissible list are :</i></b>

> <b>For Instance:</b>

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


<b>Currency:</b>  AcuBi supports following currency formats “$”, “€”, “£”, “₹”.

```
currency : currency_symbol
```
 <b>Example:</b> currency” : “$”

<b>III.</b>  <b>Time_frame:</b> AcuBi provides an option to extract different components associated with time stamp for user convenience.

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

<b>1.</b>  As a resultant of arithmetical operations done on fields of the same view.
```
"sql": "(${TABLE}.Field1 arithmetical operation ${TABLE}.Field2)"
```

>**For Instance:** 
“sql”: “(${TABLE}.Amount + ${TABLE}.Discount)”

<b>2.</b>  As a resultant of arithmetical operations done on fields of a mapped view.

```
"sql": "(${TABLE}.Field1 arithmetical operation ${Mapped_View.Field})"
```

><b>For Instance:</b>
“sql”: “(${TABLE}.Amount) / ${Customers.Total_number})”

<b>3.</b>  As a resultant of logical operations ( like case statement ) done on fields of the same view.
```
 "sql": "(case when (condition) then Expression_1 else Expression_2 end) "
```

Where condition is an expression on the fields of self view and Expression_1, Expression_2 are expressions which include fields of self view.

> <b>For Instance:</b>
 “sql”: “(CASE WHEN (${TABLE}.Name is not null) THEN ${TABLE}.Salary ELSE 0 END)”

<b>4.</b>  As a resultant of logical operations ( like case statement ) done on fields of a mapped view.

```
 "sql": "(case when (condition) then Expression_1 else Expression_2 end) "
```

Where condition is an expression defined on the fields of self view or mapped view and Expression_1, Expression_2 are expressions which include fields of self view or mapped view.

> <b>For Instance:</b> 
  “sql”: “(CASE WHEN (${[Customers.ID](http://customers.id/)} is not null) THEN ${TABLE}.Amount ELSE 0 END)”

<b>5.</b>  As a resultant of database function operated on fields.

```
   "sql": "(${TABLE}.Field * ${DB}.function_name(parameters)) "
```

> <b>Example</b>  “sql” : “(${TABLE}.Amount  KaTeX parse error: Expected 'EOF', got '​' at position 51: …te(DB.exchanger​̲ate({TABLE}.OrderDate,${TABLE}. CurrencyID))”

<b>6.</b>  As a resultant of string, date, number based sql functions on fields

```
  "sql" : "sql_function(${TABLE}.Field)"
```

> <b>For Instance:</b>
Number → “sql” : “SUM($ {TABLE}.Amount)”,  
Date → “sql” : "TO_CHAR ( $ { TABLE}.OrderDate,‘Mon-YYYY’)"  
String → “sql” : “CONCAT('Date : ',${TABLE}.OrderDate)”

<b>7.</b>  As a resultant of single value returning sql query

```
   "sql" : "(select Expression from Database.Table)"
```

Where the expression contain the fields of self view and should result a single value.
```
 “sql”: "(select sum(x.Amount) from Orders)”
```
## Time Frame Grouping

To enable grouping option for dashboard filters. Derive the following expression in model section.

```
{
"name": "whenmade",
"label": "whenmade",
"data_type": "date",
"time_frame": "hour,day,week,month,quarter,year,date",
"type": "dimension",
"lookup": "",
"operators": "",
"sql": "${TABLE}.whenmade",
"summary": "",
"visualise": "true",
"time_frame_grouping":true
}

```


## Custom View

Custom fields are user defined fields for which we apply arithmetic  and logical operations that are supported by database. A view may join other views and there relationship are defined as part of data analysis section of model file.

### New Custom View

<b>1.</b> Click on <b>New Empty view</b> to create or derive a new custom view table.

![
](https://raw.githubusercontent.com/sv18042016/fp1/cf5946b2b83468c906303fc1b8480de242f0d17b/images/New_version5/TD_Model_image10.png)
 <b><Font color = " black">Image 11</font></b>

Once the view is created, label the database field and derive the custom table using a SQL query as a result a derived table is created.
``` 
{
"name": "CustomView_2516",
	"label": "CustomView_2516",
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
			"sql": "\"CustomView_2516\".SC",
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
			"sql": "COUNT(DISTINCT \"CustomView_2516\".ORID)",
			"summary": "",
			"visualise": "true"
		},
		]
}
```
- <b>Name</b> name identifier of custom table derived.
- <b>label</b> label the custom table the way it should appear in model section. 
- <b>Info</b> provides description for custom table.
- <b>Type</b> datatype used for deriving a custom table.
- <b>Database</b> table is used to retrieve the data fields.
- <b>Connection</b> establish the database connection for deriving new fields.
## Save View

Click <b>Save</b> to Save the View in database.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/21c1e57f8188409ca0cc91dcabefc75cf50ed3be/images/New_version5/td_model_image18.png)
 <b><Font color = " black">Image 12</font></b>

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

- <b>Name</b> identifier for the field in custom table.
- <b>label</b>  the way derived field should display in custom table.
- <b>Data_type</b> define supporting parameters and string is used as  default parameter while deriving the fields for custom table.
  - <b>String</b> for measures that contain letters or special characters.
  - <b>Date</b> measures that contain dates.
  - <b>Time_frame</b> is a derived list of formats from time stamps for instance the following are the available formats hour, day, week,month,quarter, year,date,week_day, date_month, date_quarter, date_hour, year_week.
  - <b>Number</b> for the measure that contain number.
  - <b>Int</b> for the measure that contains integers.
  - <b>Type</b> can be used as part of dimension or measure.

## Lookups

- <b>lookup</b> retrieve list of values for a specific field either from database using a query or from an item list (it is listed in the filter section during visualization).
- <b>Operator</b> is used to retrieve single or multiple values in the filter section while using lookup.
 - <b>SQL</b> parameter is used to define a valid SQL expression that results in a field value.
 - <b>Summary</b> is used to retrieve the aggregate field values of the measures using the following options,
   - Sum 
   - Count
   - Average 
   - Maximum
   - Minimum

## Drill-Down 

Drill-down is used for exploring the data further with respect to a field value. AcuBi has an ability to define drill option for a field with a set of derivable fields and when clicked on a particular value of an assigned field, the individual records that make up that cell will be displayed by limiting the query with the clicked value.

## Show Drill-Down Measures

Sometimes, it may be necessary to bring the current stage measure fields to the next drill stage along with the drill fields.

AcuBi provides an additional attribute to drill down as  <b>Show drill down measures</b>  which can be defined as  <b>TRUE or FALSE</b>. If mentioned TRUE, then system will carry forward the measures of the current stage to the immediate drill level.

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
In the above example, Drill down option is defined over field “<b>State Name</b>” with two fields of self view City Name, No_of_Employees. On Clicking on any of “State Name”, then filter will be applied on that value and relevant values of fields <b>“City Name”</b> and <b>“No_of_Employees”</b> will be displayed.

As  <b>Show drill down measures</b>  is set  <b>TRUE</b>, the associated measures (if exists) of the field “State Name” will also be brought to the next stage along with drill fields City Name and No_of_Employees.


If mentioned <b>FALSE,</b> then system will not carry forward the measures of the current stage to the next drill level.
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
 “show_drill_down_measures”: “false”,  
 “visualise”: “true”  
 }

```

# Maps

Maps enables users to visualize the geographic data on reactive and interactive maps. To carry out maps  in AcuBi,Your query should include at least one dimension based on geographic data. On including measure in your query it will display the information about the location selected.

To carryout maps under visualization you need to derive the data fields in Model Section initially.

 <b>For Model, Views and for a specific field the map co-ordinates may be assigned as follows :</b>

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








<!--stackedit_data:
eyJoaXN0b3J5IjpbLTUwNTk5NCwtOTgxNDA2NzY5LC0xNjMzND
AzMzc1LC05NTk0NzM2NDcsMTM5MTcxNTkzMSw0MzI4MDI1NDUs
MjkxNjYzODYxLDIzMzcxMDAxMywxOTUzNTM2MDc3LDE1OTEyNT
UxODEsMzcyOTkwMTU1LDEyNTIwMjA3MDMsLTE0NDIzNTc2NTAs
MTAzNzEwMjExNCwtOTY5ODExNzksMTgzMTM4Njk5MSw3NTMxNT
M4NiwtMTAxMTAzMTcwOCw4ODQ3Mjc2Nyw4NDc1NTU1ODZdfQ==

-->