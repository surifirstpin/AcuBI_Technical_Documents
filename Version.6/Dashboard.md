
<center><h2>Dashboard</h2></center>

Dashboard provides access to view multiple reports in single dashboard layout, in this way it provides a quick view on related data. In order to make it more feasible to users, it is provided with set of global filters by making dashboard more interactive and can re-arrange the titles. After configuring a dashboard to your interest, you can share it with your team. You can create as many dashboards as you want, so you can alter each dashboard as per your business requirement.

## View Dashboard

To view already existing dashboard navigate to dashboard section under <b><i> My Space</i></b> list click the dashboard report you want to view.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/fa7d825c0eff00c07a5b94d7a44aac74fba8ec9c/images/New_version5/TD_Dashboard_image1.png)
 <B><font color = " Black"> Image 1 </font></b>
### Create Dashisterboard

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

-   <b>Filter Name:</B>  identifier name for the filter applicable.
    > <B>Note:</b> Filter name accepts minimum three Characters
    
-   <b>Filter Type:</b> Type of filter used (String,date,number).
    
    -   <b>String -</B>  For fields that contain letters or special characters.
        
    -   <b>Number -</b>  For fields that contain numeric values.
       
    -   <b>Date -</b>  For fields that contain dates.
        
    -   <b>Lookup - </b>  To view the lookup in dashboard filters it should be defined in lookup section.  (Refer Lookup Section)
        
    -   <b>Operator - </b> Filter operation applicable on data.
        
## LOOKUP

  <b>Lookup</b>  Adding lookup to dashboard will refer set of query or list of items in filters.
  
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/ccc11113e49adbd5fa712948a41df1f820615980/images/New_version5/TD_Dashboard_image6.png)
 <B><font color = " Black"> Image 8 </font></b>

<b>4.</b> To add new lookup to dashboard click on , Add Lookups.

-   <b>Lookup name:</b>  name of the lookup field.
    
-   <b>Lookup Type:</b>  refers to item or query type.

- <b>Connection:</b> Connection established for the query  
    
-   <b>Test Lookup:</b>  To test the lookup.
    
-   <b>Multiple Selections:</b>  Enables the selection list for multiple data. If disabled, user can select only single data.
  
  ![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/4420d6f0d9ecee55eced1d2a307bee2171c4ec1f/images/New_version5/TD_Dashboard_image11.png)  
  <b><font color = " Black" > Image 9 </font></b>


## Dependency Filters

You can refer the existing lookup, based on which a new lookup is created to retrieve the data based on referred lookup. In this way you can extract the data depending on referred lookup field.

-   <b> Referred: </b> on selecting the referred checkbox the following lookup will extract the data based on the previously created lookup for which the referred checkbox is enabled.

## Report Listeners

<b>Listeners</b> enables to register callbacks to be notified when an event is detected on a specific label. AcuBi has an ability to assign a defined filters to report column (fields of views based on which the report is created). For suppose if a filter is defined for dashboard containing 2 reports and listener is added on particular field for report 1, it is applicable only on report 1 and report 2 will remain unaffected.


![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/647c988be461bddb8f73631b10bda0beb4da5e4a/images/New_version5/TD_Dashboard_image7.png)
 <b><font color = " Black"> Image 10 </font></b>


-   <b>Dashboard Report:</b>  selects reports to add filters.
    
-   <b>Listen Filter:</b>  refers to filter option available.
    
-   <b>Apply to field:</b>  applies filter options to available field list in report.
    
- <b>Add Listener</b> adds multiple filters to reports.
    
 <b>5.</b> Click  <b>Save Button</b>  to save the dashboard.<b><i>(Refer Image 9)</i></b>

##  Privacy & Share option for Dashboards

Select tag in which you want to save  <b>Dashboard Reports</b>  and click on  <b>Save.</b> 
-   <b>Name:</b> name identifier for dashboard created.
    
-   <b>Title:</b> title to refer the dashboard.
    
-   <b>Info:</b>  summary information of the dashboard created.
    
-   <b>Privacy:</b>  you can save the report in any one of the following privacy option.
    
    -   <b>Private()</b>  It enable access for user itself.
        
    -   <b>Public()</b>  It enable access for all the users.
        
    -   <b>Share()</b>  It enable access for specific set of users.


![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/39160f7dbc8681aed71596479a2b6bb11b656289/images/New_version5/TD_Dashboard_image8.png)
 <B><font color = " Black"> Image 11 </font></b>

To view the saved dashboard open it from dashboard section and click on dashboard report name.

- it displays below screen with dashboard reports and applied global filters 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/ab627f79baffd061b5bbf8c1596bd4580c68b29c/images/New_version5/TD_Dashboard_image9.png)
  <B><font color = " Black"> Image 12 </font></b>

## Show Field Group

 Irrespective of applied global filter, on selecting checkbox <b><i>Show Field Group</i></b>, it displays list of grouped value.

## Edit / Delete Dashboard

<b>6.</b> Click  <b>Edit Button</b> to make changes to dashboard created.

> <b>Note :</b>  After editing the dashboard click on  <b><i>Save</i></b>  button to save the changes made.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/97f823b6cc1611600a983cdac5977d2a8e3cbfc7/images/New_version5/TD_Edit_Dashboard_Image1.png)
 <B><font color = " Black"> Image 13 </font></b>
 
## Delete Dashboard

<b>7.</b>  Click on  <b>Delete icon</b>  to delete the dashboard created.

  <b>8.</b> To set dashboard on home page click <b>Set Home Page</b> Icon.
  
## List View

To view the list of reports and dashboards in List View click on <b>List View.</b>

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/f7c768a770140dd07c91dc44078f61241b248d14/images/New_version5/TD_Dashboard_image13.png)
 <B><font color = " Black"> Image 14 </font></b>

## Folder View

To view the list of reports and dashboards in Folder View click <b> Folder View</b>.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/f7c768a770140dd07c91dc44078f61241b248d14/images/New_version5/TD_Dashboard_image14.png)
 <B><font color = " Black"> Image 15</font></b>

In <b>Folder View</b>, on clicking on Settings Icon, it displays <b>Info ( information given while saving any report), Edit , Delete, Thumbnail, Set Homepage</b> options for reports and dashboard. 

< Note: Tags are specific for editing, deleting and for thumbnail option.


![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/c97594b985cd884b42d5ca4c992061f338443160/images/New_version5/TD_Dashboard_image14.png)
 <B><font color = " Black"> Image 16</font></b>

## Info

 on selecting <b>Info</b> button for <b> Dashboard-->Orders</b> it will display the dashboard description window as shown in below image.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/36dbf9152ecc0c6382b569122c8e7fa15f8814ff/images/New_version5/TD_Dashboard_image15.png) 
 <B><font color = " Black"> Image 17</font></b>


## Edit 

To edit a file click on <b>Setting</b> icon and click <b>Edit</b>, it will navigate to report or dashboard you want to edit after editing the dashboard file click on save to update the changes made.
<b> For Instance: </b> Click edit for dashboard under folder view, it will navigate orders dashboard, Add new report Timeline Filters_Hd to Layout as shown in below in mage and click save to update.


## Delete

To delete a report or dashboard permanently from database click on <b>Delete</b> icon.

## Thumbnail





<!--stackedit_data:
eyJoaXN0b3J5IjpbMzM3Mzk3OTU5LC0xNzA5OTg1MjkwLC0xOD
Q1MjM0MjMyLC0xNzIyNDAxNDU3LDIwNDM3OTk4OTgsLTc0ODI3
MDg5MSwtOTg4Mzc5MTc1LDI3ODEzNTI2NiwtMTMzMDEwMzg2MC
wtMTYwNjY3MTYxNiwxNDEyOTM3NzA4LDk4ODUyMTgyOSwzOTIy
NjMyMzcsODM1NjgwNzIzLDg4MDIzMTU5NCwxMjUwMDc1MDY0LC
0yMTU5NzIyMDEsLTc0MDM0MTk2MSwxNTUwNTQ0MTI3LC0xMzQy
NDU4ODk2XX0=
-->