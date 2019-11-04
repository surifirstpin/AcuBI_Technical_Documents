


 <center><h1>SQL Runner</h1></center>

Using SQL Runner, you can directly access the database and clout it in variety of ways. In SQL Runner you can easily set up the connection, and navigate the tables under your schema.  <b>Run</b> pre-written SQL queries and view the query run history. at the same time create your customs views here and perform useful task with them in model section.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/f127fd40abc4d77b566dd8186cea91b69a9bfd25/images/New_version5/TD_SQL_Image1.png)
 <b><Font color = " black">Image 1</font></b>0

<b>Ways to create SQL queries in AcuBi</b>

<b>I.</b> Write SQL query from scratch and run the query.

 > <b>Note:</b> make sure the dialects used in SQL runner should match the database dialects.
    
<b>II.</b> Create SQL query in Reports.
    
### Steps to create SQL Query in SQL Runner

 Navigate to SQL runner by clicking on SQL Runner section.
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b39fda27ee8c1b3476ef40b62ec8a3057ff15786/images/New_version5/TD_SQL_Image2.png)
 <b><Font color = " black">Image 2</font></b>

-  Type  SQL command in SQL query area.

-   Hit the  <b>Run</b> button.

-   The data retrieved below the query area(Refer Image 2).

<b>Note:</b>  SQL runner will load up-to limit 5000 records only.

-  Click  <b>Download</b>  to download the data retrieved.

- Total <b>Numbers of Rows</b> fetched is displayed at the bottom of the screen.

-  A maximum  <b>Record limit</b>  of 5000 can be fetched at a time.
    
## SQL Runner History

To view the recent run-history and to re-run them, click on history tab available at the top right of the SQL query area. history section displays all the query run on SQL runner. <b>Green color</b> indicates query is successful and<b> Red color</b> indicates unsuccessful query due to the error.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/cc6726e8dbfc000869585b981af2b09437a7e149/images/New_version5/TD_SQL_Image4.png)

 <b><Font color = " black">Image 3</font></b>

###  Sorting Query Result

![Image 5](https://raw.githubusercontent.com/sv18042016/fp1/7ce6cf259173da9056f59348c70d063764c1ba85/images/New_version5/TD_SQL_Image4.png)
 <b><Font color = " black">Image 4</font></b>

<b>1.</b> Local Sorting can be applied directly to the data header in the result section. To enable this click on the desired field header to enable sorting.

## Find

<b>2.</b> To find the specific field value from the data extracted click on <b>Find</b> in the  field drop down.

## Group / Un-Group

<b>3.</b> By selecting group option for fields you can group the data and display the consolidated value of the field. To carry out this function click on <b>Group</b> in field drop down and <b>To release</b>the same click on <b>Un-Group.</b> 

## Pin or Remove Pin

<b>4.</b> To freeze the column field values while scrolling the data, click <b>Pin</b> in field drop down provided and to release the same click <b>Remove Pin.</b>

## Derived View

SQL Runner can create a derived view from the query build at the same time you can use this view in model section. the dialects used for creating a derived view should be same as in SQL runner.

To get started with derived view, Click on list icon and select create derived view.

![Image 6](https://raw.githubusercontent.com/sv18042016/fp1/046dbed3d1d2595b7250ed3e1c4b57ef06d76ae2/images/New_version5/TD_SQL_Image5.png)

 <b><Font color = " black">Image 5</font></b>

<b>Enter the below fields :</b>

-   <b>Derived View Name</b>  Enter Label for identification of new derived view.
    
-   <b>Projects</b>  Select the dialects using the drop down button.
    
-   <b>Query</b>  the query created in sql runner will be added here.
    
-   <b>Field List</b>  On selecting the dialects all the fields used in query are reflected here.
        
-   Click on  <b>Create,</b>  to create a new derived view.
    
    
   
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b52a0977e50ba9bf53688b5eec4c52bd9ee25087/images/New_version5/TD_SQL_Image8.png)

 <b><Font color = " black">Image 6</font></b>

To view the newly created derived view. Navigate to Model section under the view list as shown in below image.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/3cb8656e408f910d26846ad3382689421ae2e644/images/New_version5/TD_SQL_IMAGE11.png)

 <b><Font color = " black">Image 7</font></b>

## Tagged

Tagged section is used to save the pre-written query and use it later as per the business requirement.

All the created tags are visible in tagged section.  <b>Follow the below steps to create TAG:</b>

<b>5.</b> Click on <b>Tag</b>  tab, it will pop up create query Tag window :

![Image 9](https://raw.githubusercontent.com/sv18042016/fp1/1fea7f40bc70240194a4aeff0d4e11d2d69bcbfe/images/New_version5/TD_SQL_Image6.png)
 <b><Font color = " black">Image 8</font></b>

<b><i>Enter Below Information :</i></b>

- <b>Tag Name</B>  Enter tag name

- <b> Connection</b>  displays the connections established for query.

- <b>Query</b>  displays the query established.

- <b>Info</b>  enter query tag information.

-    Hit  <b>Create Tag button.</b>
 
![Image 10](https://raw.githubusercontent.com/sv18042016/fp1/f02a3a5d4407bbdc3cb6b1be6bd1654c6a7868a9/images/New_version5/TD_SQL_Image9.png)
 <b><Font color = " black">Image 9</font></b>


-   All created tags are visible under <b>Tagged Section.</b>

![Image 11](https://raw.githubusercontent.com/sv18042016/fp1/b3d9a0d4c9dd12b6dae1530c6f93a8ecd52be782/images/New_version5/TD_SQL_Image10.png)
<b><Font color = " black">Image 10</font></b>

<b>6.</b> Click on <b>Play icon</b> under tagged section to recall the saved tagged query.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/ccf284a91a406cad5b295159df179f06483cd6ee/images/New_version5/TD_SQL_IMAGE12.png)
<b><Font color = " black">Image 11</font></b>

The resultant.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/e5b86fc5839552dcfb820fbe31a379d3f506ba17/images/New_version5/TD_SQL_IMAGE13.png)
<b><Font color = " black">Image 12</font></b> 

<b>7.</b> Click <b>Delete</b> icon under tagged list to delete Query.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/213b58e85e4f6c5b77ac3d24f9a3d6951cc714ac/images/New_version5/TD_SQL_IMAGE14.png)
<b><Font color = " black">Image 13</font></b> 
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzNDc0NDEzODgsLTI2NzM3Njc2Niw1NT
A5NzY0MTYsNjMxNTk4MTYsLTIxMTEzOTcxMjgsODg1ODQ3MTY3
LDM4MDQzMDk4NSwxNzIxODYxOTYzLDI1NjMwODkzNCw4NTc5MD
Y1ODhdfQ==
-->