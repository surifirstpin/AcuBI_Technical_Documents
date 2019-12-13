
<center><h1>Dashboard</h1></center>

Dashboard provides access to view multiple reports in single dashboard layout and provides a quick view on related data. In order to make it more feasible to users, it is provided with set of global filters by making dashboard more interactive and can re-arrange the titles. After configuring a dashboard to your interest, you can share it with your team. User can create as many dashboards as you want, so you can alter each dashboard as per your business requirement.

## View Dashboard

To view already existing dashboard navigate to dashboard section under <b><i> My Space</i></b> list click the dashboard report you want to view.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/fa7d825c0eff00c07a5b94d7a44aac74fba8ec9c/images/New_version5/TD_Dashboard_image1.png)
 
 <B><font color = " Black"> Image 1 </font></b>

### Create Dashboard

> <b> Navigation : Dashboard→ New Dashboard</b>

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b41125908269765305098000fc4f2b44012ce182/images/New_version5/TD_Dashboard_image2.png) 

<B><font color = " Black"> Image 2 </font></b>

## Customize Layout

AcuBi has ability to create multiple report layouts. Depending on requirement this layout are categorized in 2 ways.

   ## Grid Layout
   
 <b>Grid Layout</b>  defines single fit layout option for reports. <b> For instance : </b> in below image we can see, i have selected Grid Layout(1 x 2) from drop down list provided for layout. <b><i>(Refer Image 3)</i></b>
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/dbd25e9b2827cdb199236be24673a440da7f8ee5/images/New_version5/TD_Dashboard_image3.png)
 
 <B><font color = " Black"> Image 3 </font></b>

## Flow Layout

 <b>Flow Layout</b>  defines multiple layout options for reports provided scroll bar. 

- To add reports in flow layout, select the grid and click on report available under <b>Workspace.</b>
- Select <b>Add</b> to add new report grid to existing layout.

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
    
    -   <b>String </B>  For fields that contain letters or special characters.
        
    -   <b>Number </b>  For fields that contain numeric values.
       
    -   <b>Date </b>  For fields that contain dates.
        
    -   <b>Lookup </b>  To view the lookup in dashboard filters it should be defined in lookup section.  (Refer Lookup Section)
        
    -   <b>Operator </b> Filter operation applicable on data.
        
## LOOKUP

  <b>Lookup</b>  Adding lookup to dashboard will refer set of query or list of items in filters.
  
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/ccc11113e49adbd5fa712948a41df1f820615980/images/New_version5/TD_Dashboard_image6.png)

 <B><font color = " Black"> Image 8 </font></b>

<b>4.</b> To add new lookup to dashboard click on Add Lookups.

-   <b>Lookup name:</b>  name of the lookup field.
    
-   <b>Lookup Type:</b>  refers to items or query type.

- <b>Connection:</b> Connection established for the query  
    
-   <b>Test Lookup:</b> it runs and verifies the lookup.
    
-   <b>Multiple Selections:</b>  Enables the selection list for multiple data. If disabled, user can select only single data.
  
  ![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/4420d6f0d9ecee55eced1d2a307bee2171c4ec1f/images/New_version5/TD_Dashboard_image11.png)  
 
  <b><font color = " Black" > Image 9 </font></b>


## Dependency Filters

You can refer the existing lookup, based on which a new lookup is created to retrieve the data based on referred lookup. In this way you can extract the data depending on referred lookup field.

-   <b> Referred: </b> on selecting the referred checkbox the following lookup will extract the data based on the previously created lookup for which the referred checkbox is enabled.

<b>For instance:</b>

In below example we are selecting referred checkbox for Lookup-1 and mention a suitable query for Lookup-2  as shown in below image.

```
select distinct orderattdid from biplus.orders where stationcode in (#stationcode#)
```
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/5c0cb1fb3a06d74036c3f2f63167997eaa485f64/images/New_version5/TD_Dashboard_image26.png)
  <b><font color = " Black" > Image 10 </font></b>
  
To view how this dependency filters works, open Dashboard report-->Filters screen.

From below image as we can see on selecting lookup stationcode-->Stationcode_2 ( which as been referred), it displays Stationcode_2 details for lookup_2 orderattdid.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/aee43eafcba340f0ecbcf189c36da0e2b34d7922/images/New_version5/TD_Dashboard_image27.png)
  <b><font color = " Black" > Image 11</font></b>
  
## Report Listeners

<b>Listeners</b> enables to register callbacks to be notified when an event is detected on a specific label. AcuBi has an ability to assign a defined filters to report column (fields of views based on which the report is created). For suppose if a filter is defined for dashboard containing 2 reports and listener is added on particular field for report 1, it is applicable only on report 1 and report 2 will remain unaffected.


![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/647c988be461bddb8f73631b10bda0beb4da5e4a/images/New_version5/TD_Dashboard_image7.png)
 
 <b><font color = " Black"> Image 11 </font></b>


-   <b>Dashboard report:</b>  selects reports to add filters.
    
-   <b>Listen to filter:</b>  refers to filter option available.
    
-   <b>Apply to field:</b>  applies filter options to available field list in report.
    
- <b>Add Listener</b> adds multiple filters to reports.
    
    ## Save Dashboard

 <b>5.</b> Click  <b>Save Button,</b> this will navigate to save dashboard window. Enter the below information in save dashboard window;

Select tag in which you want to save  <b>Dashboard Reports</b>  and click on  <b>Save.</b> 

-   <b>Name:</b> name identifier for dashboard created.
    
-   <b>Title:</b> title to refer the dashboard.
    
-   <b>Info:</b>  summary information of the dashboard created.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/39160f7dbc8681aed71596479a2b6bb11b656289/images/New_version5/TD_Dashboard_image8.png)

 <B><font color = " Black"> Image 12 </font></b>
 
##  Privacy & Share option for Dashboards
   
-   <b>Privacy:</b>  you can save the report in any one of the following privacy option.
    
    -   <b>Private()</b>  It enable access for user itself.
        
    -   <b>Public()</b>  It enable access for all the users.
        
    -   <b>Share()</b>  It enable access for specific set of users.

To view the saved dashboard open it from dashboard section and click on dashboard report name.

- it displays below screen with dashboard reports and applied global filters 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/ab627f79baffd061b5bbf8c1596bd4580c68b29c/images/New_version5/TD_Dashboard_image9.png)
  <b><font color = " Black"> Image 13 </font></b>

From above shown image we are changing global filter, by selecting all the fields (Refer image below)

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/9d6ca772337647ea123412094216ad4f2372f7a2/images/New_version5/TD_Dashboard_image22.png)

 <B><font color = " Black"> Image 14 </font></b>
 
After applying new filter values, click <b>Apply</b> button and save.  The resultant would display the data based on applied filter values as shown in image below.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/9d6ca772337647ea123412094216ad4f2372f7a2/images/New_version5/TD_Dashboard_image23.png)

 <B><font color = " Black"> Image 15</font></b>
    
## Time-Frame Grouping
 
On enabling time-frame grouping ( in Model Section ), dashboard global filters displays field grouping available for date parameters.

a. Choose grouping fields in global filter section.

b. Click on <b>Apply button</b> to apply the newly added filters.

c. Click <b>save</b> to save the changes made.

<b> Default </b>: on selecting default button it will trigger back to the previously applied filters.

> Note : similarly you can also change all the available fields in global filters

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/8c2671e29a835554b91bc7f56a8992573fcc24cf/images/New_version5/TD_Dashboard_image20.png)

  <B><font color = " Black"> Image 16 </font></b>

The resultant for the applied filters are displayed in image below.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/1e75bd88bdb6bb49d99ec1ba011c8ccb00142934/images/New_version5/TD_Dashboard_image21.png)

  <B><font color = " Black"> Image 17</font></b>


## Full Screen 

 To enable full screen for dashboard reports click list icon and select Full screen, it enables full screen for dashboard report.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/4a0a40f34ba11548fec0b86c8a6b53335c3f5f86/images/New_version5/TD_Dashboard_image28.png)
 <B><font color = " Black"> Image 18</font></b>
 
To exit Full screen, press ESC (escape) on your keyboard.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/4a0a40f34ba11548fec0b86c8a6b53335c3f5f86/images/New_version5/TD_Dashboard_image29.png)
 <B><font color = " Black"> Image 19</font></b>
 
 ## Maximize/Minimize
  
a). To maximize a report in dashboard click<b>Maximize icon </b> similarly to minimize a dashboard report hit minimize button as shown in image below.

b). Select drop-down button and choose number of rows to display in output.

c). Filter icon display under dashboard denotes filters applicable to that particular dashboard report.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/d9ba9b9b2511f182a2a490b8ad5290aaab0c14e5/images/New_version5/TD_Dashboard_image24.png)

 <B><font color = " Black"> Image 20 </font></b>

## Download CSV, CSV ; or XLXS 

To download dashboard in any of the following formats, click gear icon;
 ![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/d9ba9b9b2511f182a2a490b8ad5290aaab0c14e5/images/New_version5/TD_Dashboard_image25.png)

 <B><font color = " Black"> Image 21</font></b>
 
-   <b>Download CSV </b>  download the dashboard report in CSV format.

- <b>Download CSV; </b>  download the grouped list.

- <b>Download XLXS </b>  download the dashboard report in Excel format.

## [Refresh & Hard Refresh]

-   <b>Refresh</b>  displays the most recent data information of the report.
    
-   <b>Hard Refresh</b>  displays the most recent data information by clearing the cache for specific dashboard.
    

## List View

To view the list of reports and dashboards in List View click on <b>List View.</b>

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/f7c768a770140dd07c91dc44078f61241b248d14/images/New_version5/TD_Dashboard_image13.png)

 <B><font color = " Black"> Image 22</font></b>



## Edit  (List View)

<b>6.</b> Click  <b>Edit Button</b> to make changes to dashboard created.


![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/97f823b6cc1611600a983cdac5977d2a8e3cbfc7/images/New_version5/TD_Edit_Dashboard_Image1.png)

 <B><font color = " Black"> Image 23</font></b>

> <b>Note :</b>  After editing the dashboard click on  <b><i>Save</i></b>  button and then click update to save the changes made.

![](https://raw.githubusercontent.com/sv18042016/fp1/a927ad6ca18c7a2c729d2324f2e92f567abb0a90/images/New_version5/TD_Dashboard_image17.png)
 
  <B><font color = " Black"> Image 24</font></b>

## Delete (List View)

<b>7.</b>  Click on  <b>Delete icon</b>  to delete the dashboard created.

 <b>8.</b> To set dashboard on home page click <b>Set Home Page</b> Icon.
  
  ## Set Home Page

To set dashboard to home page click <b>Set Homepage</b>, it will navigate pop-up <b> Homepage Window</b> with success message as shown below.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/94069dc9818aca3458fd8263fd070a732be4dab3/images/New_version5/TD_Dashboard_image19.png)

<B><font color = " Black"> Image 25</font></b>

  
## Folder View

To view the list of reports and dashboards in Folder View click <b> Folder View</b>.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/f7c768a770140dd07c91dc44078f61241b248d14/images/New_version5/TD_Dashboard_image14.png)

 <B><font color = " Black"> Image 26</font></b>

In <b>Folder View</b>, Click gear Icon, it displays Info ( information given while saving any report), Edit , Delete, Thumbnail, Set Homepage options for reports and dashboard. 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/c97594b985cd884b42d5ca4c992061f338443160/images/New_version5/TD_Dashboard_image14.png)

 <B><font color = " Black"> Image 27</font></b>

## Info

 On selecting <b>Info</b> button for <b> Dashboard-->Orders</b> it will display the dashboard description window as shown in below image.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/36dbf9152ecc0c6382b569122c8e7fa15f8814ff/images/New_version5/TD_Dashboard_image15.png) 
 
 <B><font color = " Black"> Image 28</font></b>


## Edit 

To edit a file under folder view, click  <b>Gear</b> icon and  select<b>Edit</b>, it will navigate to report or dashboard you want to edit after editing the dashboard file click on save to update the changes made.

<b> For Instance: </b> Click edit for dashboard under folder view, it will navigate orders dashboard, Add new report Timeline Filters_Hd to Layout as shown in below image. 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/e12a694bb21c74293f6b391f8a81602b64454c3b/images/New_version5/TD_Dashboard_image16.png)

 <B><font color = " Black"> Image 29</font></b>

Click save then click <b>update</b> in Save dashboard window.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/a927ad6ca18c7a2c729d2324f2e92f567abb0a90/images/New_version5/TD_Dashboard_image17.png)

 <B><font color = " Black"> Image 30</font></b>
 
## Delete

To delete a report or dashboard permanently from database click on <b>Delete</b> icon.

## Thumbnail

Click on <b>Thumbnail</b> option, it will navigate to <b>Upload Thumbnail</b> window. 
  - <b>Browse :</b> Click browse button to upload image from local system.
  
  - <b> Delete :</b> Click Delete icon to delete the thumbnail.
  
  - <b>Background Color :</b> Select background color for thumbnail.
  
  - <b>Icon & Font Color :</b>  choose color for the icon using drop down list

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/3d26c0f3df14f01438f447f5b9b577478f082e84/images/New_version5/TD_Dashboard_image18.png)

<B><font color = " Black"> Image 31</font></b>




<!--stackedit_data:
eyJoaXN0b3J5IjpbNzU4NTM2MDkzLDcyNDU1MjksNzM0NTMwMj
g2LDEyODY4OTEyMTMsMTI3MTczNzM4MCwtMTU5NTE4NzM1Niwt
NzU3MDU3NTE3LDE5MzM1MjMyNDQsNTc5NzUxMzc4LDE5MjE2OD
YwNTksLTExMjM3Nzc4MzksMTk4NDEyNjczMCwtMzA3NzU3MDA0
LC00MDU2NzYzODEsNjg1OTIxNDIyLC0yMjgyOTY0ODYsLTE4Mj
IzMjY0NzYsLTEyMDU0NDUyOTgsNTU5NDc5MTA4LC00MzU5ODcx
NTBdfQ==
-->