
<center><h2>Dashboard</h2></center>

Dashboard provides access to view multiple reports in single dashboard layout, in this way it provides a quick view on related data. In order to make it more feasible to users, it is provided with set of global filters by making dashboard more interactive and can re-arrange the titles. After configuring a dashboard to your interest, you can share it with your team. You can create as many dashboards as you want, so you can alter each dashboard as per your business requirement.

## View Dashboard

To view already existing dashboard navigate to dashboard section under <b><i> My Space</i></b> list click the dashboard report you want to view.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/fa7d825c0eff00c07a5b94d7a44aac74fba8ec9c/images/New_version5/TD_Dashboard_image1.png)
 <B><font color = " Black"> Image 1 </font></b>
### Create Dashboard

> <b> Navigation : Dashboard→ New Dashboard</b>

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b41125908269765305098000fc4f2b44012ce182/images/New_version5/TD_Dashboard_image2.png) <B><font color = " Black"> Image 2 </font></b>

## Customize Layout

AcuBi has ability to create multiple report layouts. Depending on requirement this layout are categorized in 2 ways.

   ## Grid Layout
   
 <b>Grid Layout</b>  defines single fit layout option for reports. <b> For instance : </b> in below image we can see, i have selected Grid Layout(1 x 2) from drop down list provided for layout. <b><i>(Refer Image 3)</i></b>
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/dbd25e9b2827cdb199236be24673a440da7f8ee5/images/New_version5/TD_Dashboard_image3.png)
 <B><font color = " Black"> Image 3 </font></b>

## Flow Layout

 <b>Flow Layout</b>  defines multiple layout options for reports provided scroll bar. 

- To add reports in flow layout, select the grid and click <b>Add</b>  available next to report name under <b>Workspace.</b>

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/fd205f8416f11b873203f9f1915b436a996b1096/images/New_version5/TD_Dashboard_image12.png)
 <B><font color = " Black"> Image 4 </font></b>

- **Flow Layout** enables drag and drop option for the available grids, to carryout this function select <b>Drag Icon</b> and drop to desired available grid.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/0f86df89a1c0a273e0609cd6731055746e7641c7/images/New_version5/TD_Dashboard_image10.png)
  <B><font color = " Black"> Image 5 </font></b>

## Add Reports

Based on requirement multiple reports are added to layout selected.

<b>1.</b> To add reports to layout select the layout header and click on report name that you would like add, 

<b>2.</b>  To add more report layout to existing one click <b>add</b> for reports under Work space list.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/1fca98228071a251b630e285a511c3ab271a6780/images/New_version5/TD_Dashboard_image4.png)
 <B><font color = " Black"> Image 6 </font></b>

> <b>Note:</b> Use Double arrow up and Double arrow down Icon available at top right corner of dashboard screen to enable  the Global filters section.

## Dashboard Global Filters

<b>3.</b>  Click on <b>Add global filters</b>  to add global dashboard filters. 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/ccc11113e49adbd5fa712948a41df1f820615980/images/New_version5/TD_Dashboard_image5.png)
  <B><font color = " Black"> Image 7 </font></b>

-   <b>Filter Name</B>  identifier name for the filter applicable.
    > <B>Note:</> Filter name accepts minimum three Characters
    
-   **Filter Type**  type of filter used (String,date,number).
    
    -   **String**  For fields that contain letters or special characters.
        
    -   **Number**  For fields that contain numeric values.
       
    -   **Date**  For fields that contain dates.
        
    -   **Lookup**  to view the lookup in dashboard filters it should be defined in lookup section.  (Refer Lookup Section)
        
    -   **Operator**  filter operation applicable on data.
        
## LOOKUP

  **Lookup**  Adding lookup to dashboard will refer set of query or list of items in filters.
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/ccc11113e49adbd5fa712948a41df1f820615980/images/New_version5/TD_Dashboard_image6.png)
**Image 8**

**4.** To add new lookup to dashboard click on , Add Lookups.

-   **Lookup name**  name of the lookup field.
    
-   **Lookup Type**  refers to item or query type.

- **Connection** Connection established for the query  
    
-   **Test Lookup**  to test the lookup.
    
-   **Multiple Selections**  enables the selection list for multiple data. If disabled, user can select only single data.
  
  ![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/4420d6f0d9ecee55eced1d2a307bee2171c4ec1f/images/New_version5/TD_Dashboard_image11.png)  
**Image 9**

## Dependency Filters

You can refer the existing lookup, based on which a new lookup is created to retrieve the data based of the referred lookup. In this way you can extract the data depending on referred lookup field.

-   **Referred**  on selecting the referred checkbox the following lookup will extract the data based on the previously created lookup for which the referred checkbox is enabled.

## Report Listeners

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/647c988be461bddb8f73631b10bda0beb4da5e4a/images/New_version5/TD_Dashboard_image7.png)
**Image 10**

The Listeners option allows to register callbacks to be notified when an event is detected on a specific label.

AcuBi has an ability to assign a defined filters to report column (fields of views based on which the report is created). For suppose if a filter is defined for dashboard containing 2 reports and listener is added on particular field for report 1, it is applicable only on report 1 and report 2 will remain unaffected.

-   **Dashboard Report**  selects reports to add filters.
    
-   **Listen Filter**  refers to filter option available.
    
-   **Apply to field**  applies filter options to available field list in report.
    
 **Add Listener**  adds multiple filters to reports.
    
  **5.** Click  **Save Button**  to save the dashboard.(Refer Image 9)

##  Privacy & Share option for Dashboards

Select tag in which you want to save  **Dashboard Reports**  and click on  **Save.** 
-   **Name**  name identifier for dashboard created.
    
-   **Title**  title to refer the dashboard.
    
-   **Info**  summary information of the dashboard created.
    
-   **Privacy**  you can save the report in any one of the following privacy option.
    
    -   **Private()**  It enable access for user itself.
        
    -   **Public()**  It enable access for all the users.
        
    -   **Share()**  It enable access for specific set of users.


![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/39160f7dbc8681aed71596479a2b6bb11b656289/images/New_version5/TD_Dashboard_image8.png)
**Image 11**

To view the saved dashboard open it from dashboard section and click on dashboard report name.

- it displays below screen with dashboard reports and applied global filters 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/ab627f79baffd061b5bbf8c1596bd4580c68b29c/images/New_version5/TD_Dashboard_image9.png)
**Image 12**

## Show Field Group

- Irrespective of applied global filter, on selecting checkbox ***Show Field Group***, it displays list of grouped value.

## Edit / Delete Dashboard

**6.** Click  **Edit**  Button to make changes to dashboard created.

> **Note :**  After editing the dashboard click on  ***Save***  button to save the changes made.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/97f823b6cc1611600a983cdac5977d2a8e3cbfc7/images/New_version5/TD_Edit_Dashboard_Image1.png)
**Image 13**

## Delete Dashboard

**7.**  Click on  **Delete icon**  to delete the dashboard created.

  **8.** To set dashboard on home page click **Set Home Page** Icon.
  


<!--stackedit_data:
eyJoaXN0b3J5IjpbMjA2NDIzNzY5MCwtNzQwMzQxOTYxLDE1NT
A1NDQxMjcsLTEzNDI0NTg4OTYsNDY5NDgxMzM3LC04NDMxMjM5
MiwtNjE5MjI3OTQ2LDE2NDQ1ODIxMzgsLTkzNjI0NDExNywyOD
UzNzAxMjgsMTY1MzE5MjU0Niw3MzAwNDQ2MTAsMTQ1NDY3NjQz
OCw0MjM3NDUzOCwtMzYyMjQ5NzA5LDIwMjIxNzI5MjksLTE3OD
U4MzMwNzEsMTY3Njg2NDY5MSwtMzc0ODQ0NjU3LC0xMTQ1Nzc2
MTc5XX0=
-->