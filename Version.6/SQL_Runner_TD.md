


 <center><h1>SQL Runner</h1></center>

Using SQL Runner, you can directly access the database and clout it in variety of ways. In SQL Runner you can easily set up the connection, and navigate the tables under your schema.  **Run**  pre-written SQL queries and view the query run history. at the same time create your customs views here and perform useful task with them in model section.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/f127fd40abc4d77b566dd8186cea91b69a9bfd25/images/New_version5/TD_SQL_Image1.png)
**Image 1**

**Ways to create SQL queries in AcuBi**

**I.** Write SQL query from scratch and run the query.

 > **Note:** make sure the dialects used in SQL runner should match the database dialects.
    
**II.** Create SQL query in Reports.
    
### Steps to create SQL Query in SQL Runner

 Navigate to SQL runner by clicking on SQL Runner section.
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b39fda27ee8c1b3476ef40b62ec8a3057ff15786/images/New_version5/TD_SQL_Image2.png)
**Image 2**

-  Type  SQL command in SQL query area.

-   Hit the  **Run** button.

-   The data retrieved below the query area(Refer Image 2).

**Note:**  SQL runner will load up-to limit 5000 records only.

-  Click  **Download**  to download the data retrieved.

- Total **Numbers of Rows** fetched is displayed at the bottom of the screen.

-  A maximum  **Record limit**  of 5000 can be fetched at a time.

### Create SQL Query in Reports

- Navigate to Reports section, create desired report and copy paste sql query from SQL section(Reports) to SQL Runner.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/d49ce2fb758653d913874a2b3de20c2d788646fd/images/New_version5/TD_SQL_Image3.png) 
**Image 3**

-   Copy paste sql query from reports section to SQL Runner.
    
- Hit the **Run** button, You can also customize the text as per your business needs and re-run the new query.
    
### SQL Runner History

To view the recent run-history and to re-run them, click on history tab available at the top right of the SQL query area. history section displays all the query run on SQL runner. Green colour indicates query is successful and Red colour indicates unsuccessful query due to the error.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/cc6726e8dbfc000869585b981af2b09437a7e149/images/New_version5/TD_SQL_Image4.png)
**Image 4**
## Sorting Query Result

![Image 5](https://raw.githubusercontent.com/sv18042016/fp1/7ce6cf259173da9056f59348c70d063764c1ba85/images/New_version5/TD_SQL_Image4.png)
**Image 5**
**1.** Local Sorting can be applied directly to the data header in the result section. To enable this click on the desired field header to enable sorting.

## Find

**2.** To find the specific field value from the data extracted click on **Find** in the  field drop down.

## Group / Un-Group

**3.** By selecting group option for fields you can group the data and display the consolidated value of the field. To carry out this function click on **Group** in field drop down and **To release** the same click on **Un-Group**. 

## Pin or Remove Pin

**4.** To freeze the column field values while scrolling the data, click **Pin** in field drop down provided and to release the same click **Remove Pin.**

### Derived View

SQL Runner can create a derived view from the query build at the same time you can use this view in model section. the dialects used for creating a derived view should be same as in SQL runner.

To get started with derived view, Click on list icon and select create derived view.

![Image 6](https://raw.githubusercontent.com/sv18042016/fp1/046dbed3d1d2595b7250ed3e1c4b57ef06d76ae2/images/New_version5/TD_SQL_Image5.png)

**Image 6**

**Enter the below fields :**

-   **Derived View Name**  Enter Label for identification of new derived view.
    
-   **Projects**  Select the dialects using the drop down button.
    
-   **Query**  the query created in sql runner will be added here.
    
   -   **Field List**  On selecting the dialects all the fields used in query are reflected here.
        
    -   Click on  **Create,**  to create a new custom view.
    
    
   
![Image 7](https://raw.githubusercontent.com/sv18042016/fp1/0d200b374d05d63387cd4b7b0b84be4713ac6f8a/images/New_version5/TD_SQL_Image8.png)
**Image 7**

To view the newly created derived view. Navigate to Model section under the view list as shown in below image.


![Image 8](https://raw.githubusercontent.com/sv18042016/fp1/51255d3dbab14ac3607ff6091c095452be43d238/images/model_derived_view.png)
**Image 8**


## Tagged

Tagged section is used to save the pre-written query and use it later as per the business requirement.

All the created tags are visible in tagged section.  **Follow the below steps to create TAG:**

**5.** Click on **Tag**  tab, it will pop up create query Tag window :

![Image 9](https://raw.githubusercontent.com/sv18042016/fp1/1fea7f40bc70240194a4aeff0d4e11d2d69bcbfe/images/New_version5/TD_SQL_Image6.png)
**Image 9**

***Enter Below Information :***

- **Tag Name**  Enter tag name

- **Connection**  displays the connections established for query.

- **Query**  displays the query established.

- **Info**  enter query tag information.
 
 - Hit  **Create Tag button.**
 
![Image 10](https://raw.githubusercontent.com/sv18042016/fp1/f02a3a5d4407bbdc3cb6b1be6bd1654c6a7868a9/images/New_version5/TD_SQL_Image9.png)
**Image 10**

-   All created tags are visible under  **Tagged Section.**

![Image 11](https://raw.githubusercontent.com/sv18042016/fp1/b3d9a0d4c9dd12b6dae1530c6f93a8ecd52be782/images/New_version5/TD_SQL_Image10.png)
**Image 11**
<!--stackedit_data:
eyJoaXN0b3J5IjpbOTQ2MzkwMTBdfQ==
-->