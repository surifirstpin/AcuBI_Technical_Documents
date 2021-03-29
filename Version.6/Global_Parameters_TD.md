


<h1><center> Global Parameter</center></h1>

Global Parameter is a flat file data in JSON format which can be used to manipulate, control and set predefined values. AcuBi allows you to provide additional key values to manipulate the data in calculations column, control data etc.

## Standard Functionalities

-   Control data access based on login.
-   Provide access to predefined list of filter values based on login.
-   Manipulate data with external parameter based on a common reference.
-   View and manipulate data based on login.
-   Use global parameters in calculated column to perform mathematical calculations on existing data.

## Create Global Parameters

<b>Navigation : Settings → Global Parameters.</b>

<b>1.</b>  Click on  <b>Add Key.</b>

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/46f96dc3b59ecd850ed2e7bfd6bbc0e114adc902/images/New_version5/TD_Gobal_Parameter_Image1.png)
 <b><font color = "black">Image 1</font></b>

-   Enter  <b>key name</b>  as shown in the pop-up screen below, then Click on  <b>OK</b>  button.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/cff8a30a919544c66b3de1e567ed807c04e49ace/images/New_version5/TD_Gobal_Parameter_Image14.png)
 <b><font color = "black">Image 2</font></b>

-   Click on  <b>Add column</b>  to add table data ( strings or Numbers).
    
-   Click on  <b>Add Row</b>  to increase the table rows.

   ![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/cff8a30a919544c66b3de1e567ed807c04e49ace/images/New_version5/TD_Gobal_Parameter_Image6.png)
 <b><font color = "black">Image 3</font></b>

<b>2.</b>  Click on <b>Browse Button</b> to import the file.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/74c4003c8e1e7bdf8c8b99468ba07dcfaf0596a8/images/New_version5/TD_Gobal_Parameter_Image4.png)
 <b><font color = "black">Image 4</font></b>

After importing the file, data is reflected in global parameter section. <b>(Refer Image 5)</b>

<b>3.</b>  Click on  <b>Save</b>  button to save the global parameter.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/8b7bd890c01292d127bb19bab0e64287df164c35/images/New_version5/TD_Gobal_Parameter_Image9.png)
 <b><font color = "black">Image 5</font></b>

> <b>Note :</b>  By default all the columns in uploaded file will be saved as string type.

## Find

<b>4.</b> To find specific cell value in global parameter click on field column header drop-down and select find. Then enter the desired cell value.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/8b7bd890c01292d127bb19bab0e64287df164c35/images/New_version5/TD_Gobal_Parameter_Image10.png)
 <b><font color = "black">Image 6</font></b>

## Edit

<b>5.</b>  Select the column name and click on  <b>Edit</b>  button to change column name and column type ( string or number using drop down list).

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/855ff834d3525786d6a8240825f529a25d6c95f2/images/New_version5/TD_Gobal_Parameter_Image11.png)
 <b><font color = "black">Image 7</font></b>


## Delete

<b>6.</b>   Similarly you can delete the column or row by selecting delete option in drop down list.

<b> Note:</b> <i>Similarly edit column cell value by clicking on specific cell as shown below:</i>

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/6d8887dfd4a991b567c8c23b558446081c24e50f/images/New_version5/TD_Gobal_Parameter_Image12.png)
 <b><font color = "black">Image 8</font></b>


## Grid & Code Views

<b>7.</b> <b>Code view</b> is used to display <b>JSON</b> format for uploaded file.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/30d986cd1364cb534c9f670a6b1f2947c2d39d40/images/New_version5/TD_Gobal_Parameter_Image13.png)
 <b><font color = "black">Image 9</font></b>

<b>Note :</b>
-   To undo the changes done for the code established click  <b>Undo</b>  icon.
-   To redo the changes done for the code click  <b>Redo</b>  icon.
-   To format the code according to proper alignment click <b>Format Code</b>  Icon.

## Check Case Functionality On / Off

If check case is enabled, global parameters become case sensitive for key mapping in calculated column.

## Global Keys

<b>Functionality : </b>Through Global Parameters we can run cluster of jobs using Global Params and this Global params are reused in many jobs .

  

<b>Interpretention : </b> Always editing the jobs and changing the dates leads to failure of job. So to overcome this situation we are calling the date functionalities through Global parameters .This Global Params which are created are used in Job and called through Block From and Block To. This interface enables you to avoid opening and editing the file. As a result the application saves your

time and helps you avoid accidental errors.

  

  

**1.** Go to Settings→Global Parameters and click on Add Key to give Key Name.

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/GP1.png?raw=true)
 <b><font color = "black">Image 1</font></b>


**2.** By selecting above Key Name click on **Add Column** and **OK**

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/GP2.png?raw=true)
 <b><font color = "black">Image 2</font></b>


**3.** Now by selecting above Key Name click on another **Add Column** and **OK**

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/GP3.png?raw=true)
 <b><font color = "black">Image 3</font></b>


**4.** Double click on underneath the Blockfrom and Blockto to mention the required date formats to save.
![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/GP4.png?raw=true)
 <b><font color = "black">Image 4</font></b>

**5.** Now through jobs we need to call the global parameters. By using #KeyName.ColumnName we mention this format in Block From and Block To as shown in below image.

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/GP5.png?raw=true)
 <b><font color = "black">Image 5</font></b>
 
**6.** Finally save the job and in case if the date needs to be changed can navigate to Global Parameters for further use.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTk4MTkzNzY2LC03NTI4MzI5NzgsMTk3OD
I5NTIxMiw1NzAzNDM2NjMsLTE5NTE1MzQ3MDIsMTU1OTIxNzU5
OSwtNDQ1NTc4NzAwLC05MzE4NzM1MzgsLTMyMzI1OTEwNiwtOD
M2NDIzNDI3LC0xMDA3OTM3NTk3LDIwNjk1NzY3MjEsNzMyMjY2
OTEzLDEyODU5ODQwMjcsOTMzODQyNjUsNDU2NDUyNTA2LC0yMD
I5ODM1NjA0LC0xMTgwMDM3ODI4XX0=
-->