
<center><h2>Dashboard</h2></center>

Dashboard provides access to view multiple reports in single dashboard layout, in this way it provides a quick view on related data. In order to make it more feasible to users, it is provided with set of global filters by making dashboard more interactive and can re-arrange the titles. After configuring a dashboard to your interest, you can share it with your team. You can create as many dashboards as you want, so you can alter each dashboard as per your business requirement.

## View Dashboard

To view already existing dashboard navigate to dashboard section under ***My Space*** list click the dashboard report you want to view.

-   To edit a tag click ***edit*** icon.
  - To set Thumbnail for a tag click ***Thumbnail*** icon.
 - Tags can be saved in Public, Private or Share under ***sharing status.*** 
-   To delete a tag click ***delete*** icon.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/fa7d825c0eff00c07a5b94d7a44aac74fba8ec9c/images/New_version5/TD_Dashboard_image1.png)**Image 1**

### Create Dashboard

> **Navigation : Dashboard→ New Dashboard**

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b41125908269765305098000fc4f2b44012ce182/images/New_version5/TD_Dashboard_image2.png)**Image 2**

## Step 1: Customize Layout

AcuBi has ability to create multiple report layouts. Depending on requirement this layout are categorized in 2 ways.

-   **Flow Layout**  defines multiple layout options for reports provided scroll bar.
    
-   **Fixed Layout**  defines single fit layout option for reports
    
 Here for instance i am choosing Grid Layout(1 x 2) from drop down list provided for layout. (Refer Image 2)
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/dbd25e9b2827cdb199236be24673a440da7f8ee5/images/New_version5/TD_Dashboard_image3.png)
**Image 3**

## [Step 2: Add Reports]

Based on requirement multiple reports are added to layout selected.

- To add reports to layout select the layout header and click on report name that you would like add, 
- To add more report laypou

**4.**  Click  **Update Report**  to add reports to layout. You can add reports to layout in 2 ways.(refer image 4)

**a.**  Click on report layout section then select the report you want to add in layout.

**b.**  Click  **Add**  to add new layout to existing one.

![
](https://raw.githubusercontent.com/sv18042016/fp1/dd00678604bb2220939239b3abcd5e2e359936b3/images/dashboard_layout.png)

**Image 4**

## [Step 3: Dashboard Global Filters](http://18.196.122.102/documentation/bi_technical_documentation.html#/Dashboard?id=step-3-dashboard-global-filters)

**5.**  Click on  **Apply Filters**  to add global dashboard filters and lookups.  **(Refer image 4)**

**6.**  **Dashboard global Filters**  allows user to view limited data by applying filters on dashboard reports.  **(Refer Image 5)**

-   **Filter Name**  identifier name for the filter applicable.
    
-   **Filter Type**  type of filter used (String,date,number).
    
    -   **String**  For fields that contain letters or special characters.
        
    -   **Number**  For fields that contain numeric values.
        
    -   **Date**  For fields that contain dates.
        
    -   **Lookup**  to view the lookup in dashboard filters it should be defined in lookup section.  **( Refer point 7)**
        
    -   **Operator**  filter operation applicable on data.
        

**7.**  **Lookup**  Adding lookup to dashboard will refer set of query or list of items in filters.**( Refer image 5)**

-   **Lookup name**  name of the lookup field.
    
-   **Lookup Type**  refers to item or query type.
    
-   **Test Lookup**  to test the lookup.
    
-   **Multiple Selections**  enables the selection of list for multiple data.
    

## [Dependency Filters](http://18.196.122.102/documentation/bi_technical_documentation.html#/Dashboard?id=dependency-filters)

You can refer the existing lookup, based on which a new lookup is created to retrieve the data based of the referred lookup. In this way you can extract the data depending on referred lookup field.

-   **Referred**  on selecting the referred checkbox the following lookup will extract the data based on the previously created lookup for which the referred checkbox is enabled.

**8.**  **Report Listeners**  **( Refer image 5)**

The Listeners option allows to register callbacks to be notified when an event is detected on a specific label.

AcuBi has an ability to assign a defined filters to report column (fields of views based on which the report is created). For suppose if a filter is defined for dashboard containing 2 reports and listener is added on particular field for report 1, it is applicable only on report 1 and report 2 will remain unaffected.

-   **Dashboard Report**  selects reports to add filters.
    
-   **Listen Filter**  refers to filter option available.
    
-   **Apply to field**  applies filter options to available field list in report.
    
-   **Add Listener**  adds multiple filters to reports.
    

**9.**  Click  **Save Button**  to save the dashboard  **( Refer image 5).**

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/ac1da552c0d05c08fa1aad5c0c1d07df190fd388/images/dash_filters.png)**Image 5**

## [Step 4: Privacy & Share option for Dashboards](http://18.196.122.102/documentation/bi_technical_documentation.html#/Dashboard?id=step-4-privacy-amp-share-option-for-dashboards)

Select the tag in which you want to save  **Dashboard Reports**  and click on  **Save.**  **(Refer image 6)**

-   **Name**  name identifier for dashboard created.
    
-   **Title**  title to refer the dashboard.
    
-   **Info**  summary information of the dashboard created.
    
-   **Privacy**  you can save the report in any one of the following privacy option.
    
    -   **Private()**  It enable access for user itself.
        
    -   **Public()**  It enable access for all the users.
        
    -   **Share()**  It enable access for specific set of users.
        

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/0fb2c0fe9fbc99b6ac2cd3d818fe7533a74872b8/images/2018-02-06_16-09-56.png)**Image 6**

## [Edit / Delete Dashboard](http://18.196.122.102/documentation/bi_technical_documentation.html#/Dashboard?id=edit-delete-dashboard)

**10.**  Click  **Edit**  Button to make changes to dashboard created.

> **Note :**  After editing the dashboard click on  **update**  button to save the changes made.

**11.**  Click on  **Delete icon**  to delete the dashboard created.

**12.**  To create a new dashboard report click on  **New Dashboard**  icon.

**13.**  To set dashboard to full screen, Choose  **Full screen**  from the list.

> **Note :**  You can also edit, delete or create new dashboard using  **Bars icon**

![
](https://raw.githubusercontent.com/sv18042016/fp1/5b86a054406ca26550a23a1c524c998d71b60505/images/dashboard_fullscreen.png)**Image 7**

## [Dashboard for Mobile Device](http://18.196.122.102/documentation/bi_technical_documentation.html#/Dashboard?id=dashboard-for-mobile-device)

AcuBi, makes it easier to view the dashboard list in mobile devices easily and displays the following features;

-   Displays dashboard list.
-   Displays dashboard report data.
-   You can add more filters to report.

![
](https://raw.githubusercontent.com/sv18042016/fp1/a11e40d845baa1742caa99ef8bec4ed3db8eed14/images/mobile_device.png)
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTU1NDQ2MTQ3MywzNjI1NjM5MywxNjA2Nj
UxOTY1LDEyNjY3OTEyNzYsMTg2NTM3MjI3LDYxMDYwOTE0M119

-->