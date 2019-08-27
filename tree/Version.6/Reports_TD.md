
<center><h2>Reports</h2></center>

<b>Reports</b> are the starting point for building a query.  it is designed in such a way, that it retrieves the data in desired combinations as per your business needs and explores particular subject area it self. It also provides an ability on how to pull the data and how to modify the report and drill down deeper into the report for more insight.
 
<b><i>Let see in detail, How AcuBi helps you in retrieving the data as per your business needs :</i></b>
 
<b>1.</b> Click on <b>Reports Section</b> and select the desired <b>Project</b> and <b>Model</b> based on which the data is retrieved.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b743a83f523e1d6ddfc4593b9e04d0f6abe03e5e/images/New_version5/TD_Reports_1.png)
 <b><Font color = " black">Image 1</font></b>

- To create a new report click on <b>Reset Visualization</b> ( refresh icon).

## Adding Dimension and Measure

A <b>Dimension</b> is a group of data and <b>Measure</b> is information about group of data and they collectively acts as fundamental building blocks for a query.

> <b>For Instance :</b> <b>Name of the Employee</b> is defined as dimension and <b>Salary of the Employee</b> is defined as Measure.
 
 <b><i>To retrieve the data in report section follow the below steps,</i></b>
 
<b>2.</b>  Select one or more dimension fields ( Grey fields) to access the data. It supports strings and date types.

<b>3.</b> Select one or more measure fields (Orange fields) to access numeric values, such as Sum, Count, Max, Min and  Avg etc. (Refer Image 1)

  > <b>Note :</b> To hide Explore/Visualize sections  click on  <b>angle double left</b> icon. To display the same click <b>angle double right  (»)</b> icon available above dimensions and measure field list.

                                                                                                                                                                                                                    
## Filters 

Filters  in AcuBi pull out the data by displaying the filtered information from database. Filters are the advanced way to limit the data. 

<b><i>The following are the various types of filter expressions used:</i></b>

| Type | Description |
|--|--|
| String | For fields that contain letters or special characters |
|Numbers|For fields that contain numeric values|
|Date|For fields that contain dates|
|Lookup| To view the lookup in Report filters it should be derived first under lookup field, in model section|

## Filters characteristics applicable :

### String:
|			Example            |						Description                        |                                                                                 
|------------------------------|-----------------------------------------------------------|
|is not null                   | should not be equal to null                               |
|is null                       | equal to null                                             |
|is not empty                  | should not be empty                                       |
|is empty                      | should be empty                                           |
|equal                         | should be equals to specific value                        |
|not equal                     | shouldn't be equal to specific value                      |
|in                            | selection based on combination of filter values           |
|not in                        | excluding set of values                                   |
|begins with                   | finds any value that starts with mentioned sub-string      |
|doesn’t begins with           | finds a value that doesn't begin with mentioned sub-string|
|Contains                      | contains mentioned sub-string                             |
|doesn’t contain               | finds a value which does not contain mentioned sub-string |
|ends with                     | should end with mentioned sub-string                      |
|doesn’t end with              | should not end with mentioned sub-string                  |

### Integer:

|			Example            |						Description                         |                                                                                 
|------------------------------|------------------------------------------------------------|
|is not null                   | should not be equal to null value                          |                
|is null                       | should be equal to null value                              |                                           
|not empty                     | data is not empty                                          |
|is empty                      | data is empty                                              |
|equal                         | data equal to specified value                              |
|not equal                     | data not equal to specified value                          |
|in                            | data equal to specified values                             |
|not in                        | data not equal to specified values                         |
|less                          | data less than specified value                             |
|less or equal                 | data less than or equal to specified value                 |
|greater                       | data greater than specified value                          |
|greater or equal              | data greater than or equal to specified value              |
|between                       | data in between the specified range                        |
|not between                   | data not in between the specified range                    |

### Date:

|			Example            |						Description                         |                                                                                 
|------------------------------|------------------------------------------------------------|
|timeline                      |data from specific time scale                               |
|equal                         |data from specific date                                     |
|not equal                     |data excluding from specific date
|between                       |data in between the specified dates
|not between                   |excluding the data between the specified range
|less or equal                 |data up to specified date 
|greater or equal              |data from the specified date 
|is not null                   |data which is not equal to null
|is null                       |data which is equal to null

> <b>Note :</b> For more details on <b>Timeline Filters,</b> Refer timeline filters document.

<b>4.</b> Navigate to <b>Filter section</b>, then extract data based on filters applied.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/eb353d0308368c774c84058005a471ff667e7125/images/New_version5/TD_Reports_2.png)
 <b><Font color = " black">Image 2</font></b>

## Hidden Filters

The data is retrieved based on hidden filters applied, this applied hidden filter fields are not visible in data section they are only visible under filter expression list.

<b><i><u>To carry out this function, follow the below steps:</u></i></b>

<b>a.</b>  Apply hidden filters to dimension.(Start_date_month)

<b>b.</b> Fields to which hidden filters applied are visible in filter expression of filter section.

<b>c.</b> The data is retrieved, based on the applied hidden filters.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/1f4b77c16dbb8f5b7ff70eb159ddb35c6445236c/images/New_version5/TD_Reports_3.png)
 <b><Font color = " black">Image 3</font></b>

- To add more filters click <b>Add Rule.</b>

- To delete the filter applied click <b>Cross Icon.</b>

- To hide the <b>Filter</b> or <b>Order</b> section Click on angle-double-up icon on to far right of the order section. To un-hide click on angle-double-down icon at same location.

<b>5.</b> Hit the <b>Run</b> button to display the data based on applied filters.

## Order  (Ascending / Descending)

To view the column data in ascending or descending orders, Click <b>Order</b> and choose the fields with desired combination, resulting on which the result in data section is displayed.
as shown In the below image, descending order is applied to bets_usd (sum), the resultant for this is shown in descending order.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/34680d9c76d6eebc3cc6b1bb76af169b96af03c3/images/New_version5/TD_Reports_4.png)
**Image 4**

## Local Sorting

Local Sorting can be applied directly to the data obtained for dimension and measure fields in the data section. To enable this click on the desired field header to enable sorting.

For <b>Dimensions</b>

- Click Upwards pointing arrow, to enable  ascending order.
- Click Downwards pointing arrow, to enable descending order.  

For <b>Measures</b>

- Click Upwards Pointing Arrow,  to enable descending order.
- Click Downwards Pointing Arrow, to enable ascending order.
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/87a73aeac27bf279f1b6a9d87a473785644d363f/images/New_version5/TD_Reports_5.png)
 <b><Font color = " black">Image 5</font></b>

## Query Time

<b>6.</b> Display total time taken to build the query of a report.

## Display number of rows

<b>7.</b> Display number of rows fetched while retrieving data.

## Display Totals

<b>8.</b>    On selecting  <b>Check box</b> for totals, the report is displayed with total sum values of the measure fields obtained.

 ## Display  Row Limit

<b>9.</b>  You can limit the rows extracted to 100, 500, 1000, 5000, etc. By selecting the limit value to your desired number from drop down list.                                                          

<b>10.</b> To download the data in csv format, click <b>download data</b>.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/1877afffe878ada04f7e66846fc1f74161830c79/images/New_version5/TD_Reports_6.png)
 <b><Font color = " black">Image 6</font></b>

## Pivot table

Multiple dimensions in report data are often easier to look at, when you pivot one of the dimensions horizontally and display group based data for the field to which pivot is applied. 
To <b>Pivot</b> a dimension click on pivot for dimension before or after running the query.

> <b>Note :</b> you can add more pivots to other dimension fields but make sure you have at least one un-pivoted dimension and a measure value.

<b>For instance,</b> To view number of orders received based on the month it displays in following way:

| Order Received  |year  |month|Region|Name|
|--|--|--|--|--|
|100 |2000|January|north|john|
|200|2001|February|south|Steve|
|300|2002 |march|east|Bob|
|400|2003|April|west|Mecker|

On Applying pivot on month, it displays;
  
|January|February|March|April|
|--|--|--|--|
|100|200|300|400|
|2000|2001|2002|2003|
|North|south|east|west|
|john|Steve|bob|Mecker|

 <b>You can apply pivot to fields in 2 ways :</b>
 
<b>a.</b> Apply pivot <b>After Retrieving</b> the data by selecting the pivot in drop down of the field.
 
<b>b.</b> Apply pivot <b>Before Retrieving</b> the data while selecting the fields by clicking on pivot icon.
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/eed95c0e5c6888ef680626c8f9e22a7ad38c9125/images/New_version5/TD_Reports_7.png)
 <b><Font color = " black">Image 7</font></b>

## Hide data in pivot 

To hide first column of pivoted data  in visualization, choose pivot hide first, to hide the last column data, choose pivot hide last in data section under data sets.


## Pin or Remove Pin

<b>11.</b> To freeze the column field values while scrolling the data, click <b>Pin</b> in field drop down provided and to release the same click <b>Remove Pin.</b>

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/e3b108aa27ba503adc4f5e185cee2743d7094208/images/New_version5/TD_Reports_8.png)
 <b><Font color = " black">Image 8</font></b>

## Group / Un-Group

<b>12.</b> By selecting group option for fields you can group the data and display the consolidated value of the field. To carry out this function click on <b>Group</b> in field drop down and <b>To release</b> the same click on <b>Un-Group.</b>



![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/bc9bcd938189cd95f72d69d632d643df0746e9af/images/New_version5/TD_Reports_9.png)
 <b><Font color = " black">Image 9</font></b>

## Multi-Level grouping

To carry out Multi-level grouping. Apply group to any of the 2 dimension fields.

> <b><i>For instance:</i></b>  In the below image grouping has been applied to dimension fields <b>customer and hub.</b> In data retrieved below on expanding HUB it displays the perspective CUSTOMER that belonging to specific hub, on further expansion it displays Casino name.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/0b15f99af3dde5ba74467811bdd3ff84e8ae541b/images/New_version5/TD_Reports_10.png)
 <b><Font color = " black">Image 10</font></b>

## Find

<b>13.</b> To find the specific field value from the data extracted click on <b>Find</b> in the  field drop down. (Refer Image 8)

## Field Visualization On / Off

<b>14.</b> To hide the specific field in the visualization charts click on <b>Hide Visualization</b> in the drop down of field  and to display the same click on <b>Show visualization.</b>(Refer Image 8)


## Remove

<b>15.</b> To remove a specific field column from the extracted list click on <b>Remove</b> in drop down list of the field.(Refer Image 8)

##  Reordering Column

To reorder columns in the <b>Data</b> section by clicking on column header and moving it to desired position. the visualizations section will reflect the new column order after hitting the <b>Run</b> button.



You can reorder columns in the  **Data**  section by clicking on a column header and moving the column to its desired position. The Explore’s visualization will reflect the new column order after you click  **Run**.

Columns are organized in the  **Data**  section by field type: dimensions, dimension  [table calculations](https://docs.looker.com/exploring-data/using-table-calculations), measures, measure  [table calculations](https://docs.looker.com/exploring-data/using-table-calculations), and  [row totals](https://docs.looker.com/exploring-data/exploring-data#displaying_totals). Columns can be reordered within each field type but cannot be moved out of their field type section. For example, dimension table calculations can be rearranged among themselves, but you cannot place a dimension table calculation in between two measures.

Columns under a pivoted dimension can be reordered, but the order of pivoted dimensions can only be changed by changing the sort order, not by manual reordering.

If your Looker admin has enabled the  [Table-Next](https://docs.looker.com/exploring-data/visualizing-query-results/table-next-options)  Labs feature, there are  [additional options](https://docs.looker.com/exploring-data/visualizing-query-results/table-next-options#manually_moving_and_pinning_columns)for reordering columns in the table-next visualization.

## Calculated Column 

Table calculations enable you to easily create on-the-fly metrics, which are similar to formulas found in Excel sheets. These extracted columns will show up in green color in data table. Using calculated column you can perform mathematical, logical (true/false), lexical (text-based), and date-based calculations on the dimensions, measures, and other table calculations in your query. 

Click on <b>Calculated Column</b> button to enable table calculations as shown in image below,

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/96a6c4d7d9cd243bc1742d6a45a3372d87704877/images/New_version5/TD_Reports_11.png)
 <b><Font color = " black">Image 11</font></b>

- <b>Field name</b> unique identifier name to refer calculated column.

- <b>Label</b> labeling the calculated column.

- <b>Data type</b> data type used (string,number).

- <b>Field type</b> derives dimension or measure.

- <b>Calculation</b> derive arithmetical & logical expressions.

- <b>Calculate on the raw data</b> if it is enabled the calculation is applied on all rows irrespective of grouping and pivot, if disabled calculation applied on abstract values.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/c80c47106a0f82196eaeb00516008a3e4c34e395/images/New_version5/TD_Reports_12.png)
  <b><Font color = " black">Image 12</font></b>

Click <b>OK</b> after deriving the expression,  all the values based on calculation is shown up in green color. (Refer Image 13)

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/2650b28af1c38a1025bbf8318c0a67dbb93dac11/images/New_version5/TD_Reports_13.png)
  <b><Font color = " black">Image 13</font></b>
> Note: for In depth information about calculated column, kindly navigate to Calculated Column Document.


## SQL Query 

To View the SQL query built on retrieving data in report, click on <b>SQL section.</b>

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/e89fea59c7b6d6978b5430de4d1be5cbfe27aeb3/images/New_version5/TD_Reports_15.png)
 <b><Font color = " black">Image 14</font></b>

## Drill Down Display

Using drill down you can view more deeper insights of the data. To enable this feature we need to define following code in Model section under prescribed project fields.

>   <b><i>Note 1:</i></b> For " TRUE " option it will display both dimensions and measure field.

```
{
			
			"name": "stationcode",
			"label": "stationcode",
			"data_type": "string",
			"type": "dimension",
			"lookup": "",
			"operators": "",
			"sql": "${TABLE}.stationcode",
			"summary": "",
			"drill_down_fields": "wayused,areacode",
			"show_drill_down_measures": "true",
			"visualise": "true"
		
		},
```


![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/a5605d5be15fd6fba7dfd3e99698cdee7b76a553/images/New_version5/TD_Reports_18.png)

  <b><Font color = " black">Image 15</font></b>


><b><i>Note 2: </i></b> Similarly For False, it will display only dimension fields.

```
	{
			"name": "stationcode",
			"label": "stationcode",
			"data_type": "string",
			"type": "dimension",
			"lookup": "",
			"operators": "",
			"sql": "${TABLE}.stationcode",
			"summary": "",
			"drill_down_fields": "wayused,areacode",
			"show_drill_down_measures": "false",
			"visualise": "true"
		},
```




<b>For example:</b> (Consider Image 15)

<b>a.</b> On expanding Station Code, it will display Station code details (eg: area code, way used & quantity)  that fall under the particular station_2.

<b>b.</b> On further expanding Way
used (Phone) for area code SS_z2, it will display the Phone numbers that fall under this particular area code.

- <b>Reset Data Drill:</b> To navigate to  previous page click <b>Rest Data Drill.</b>

> <b>Note :</b> To attain drill down features it need to be specified in model section, refer <b>Model Documentation</b> for more information about drill down feature.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjc0NjM4MDkzLDE2NTU4Nzc0NzcsNzE3Mj
g1Mjc2LC05NTAxNDk2ODksLTE1MzEzMTU4MTUsLTEyNDUwMzUw
NjksOTk3MTM5OTA3LC0xMjY4ODA1ODMzLDU5NTY3MjMxMywtNj
c0NDU5NDI1LC0xNTY4MjQxMTIzLC0xNzc1MDQwNjU3LC0yNjA5
MjE5NywtMTk1Njc5MjkzMiwtMjA0NjU3ODY3MywtMTgyNTQ5MD
IwLDgxODYxMTMzOSwtNjA2Mzc0MjU3LC00NjEwMzIwMzMsMTkz
NzM3NzIxXX0=
-->