

<center><h1>Visualization</h1></center>


<b>AcuBi</b> has an ability to create graphics and charts based on the result obtained. Charts sections in AcuBi displays different type of pictorial representation of the data.

<b>Let us see in details how to configure visualization;</b>

Reports fetches an impressive and good looking charts with the data obtained, in fraction of seconds.
 
## Getting Started With Visualization.

Click on <b>Charts</b> tab to configure visualization option for the result obtained. This will connect you to visualization section.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/52de5df82ef6986d3c2224728e8100490c41ad22/images/New_version5/TD_Visu_Image1.png)
<b><font color = "Black"> Image 1</b>


## Types of Visualization

AcuBi visualization charts are used based on the priority of what specific information you want to view about the data retrieved. Each type of visualization have different setting which can be customized for its appearance. It Provides an ability to visualize the data in 11 different types of charts with some standard editing options. 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/0dc367172608197f5a129c93f4c0c2992c7bb50c/images/New_version5/TD_Visu_Image2.png)
<b><font color = "Black"> Image 2</b>

<b><i> Let us see them in detail : </i></b>
 - Line
 - Horizontal Bar
 - Pie
 - Radar
 - Widget
 - Bar
 - Bubble
 - Table 
 - Funnel
 - World

<b><i>Let us see in detail how this charts works;</i></b>

## Line Chart

 Line chart emphasize the overall shape of an entire series of values, usually over time.
 
 <b>1.</b> Choose chart type <b>LINE</b> from given drop-down list compare the data using line chart.
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/a423f24e45a87ceabf95d366b4f659dc468ce1b4/images/New_version5/TD_Visu_Image3.png)
<b><font color = "Black"> Image 3</b>

 ### General Editing Options Specific to Line Chart
 
 - <b>Line type</b> displays the information as a series of data points called markers. Below are the list of markers used in line chart ( spline acts as  default line type), 
   - Line
   - Spline 
   - Step
   - Area
   - Area-Spline
   - Area-Step
   - Scatter
    
- <b>Points</b>  will display the data by specifying the points on the chart.

- <b>Point style</b> will specify how the data points will appear on chart. 
Below are the following point styles available in AcuBi. 
  - Circle
  - Triangle
  - Rectangle
  - RectRot
  - Cross
  - CrossRot
  - Star
  - Line
  - Dash

## Horizontal Bar Chart 

Horizontal Bar charts are used to compare data across different categories horizontally. You can build a bar chart by placing a dimension on the Y-axis and a measure on X-axis.

 <b>2.</b> Choose chart type <b>HORIZONTAL BAR</b> from given drop-down list compare the data using horizontal chart.
 
- <b>Stacked (Data)</b> Series of values are added on the Y-axis by displaying  each consecutive values above the last. 

- <b>100% Stacked (Data)</b>  Series of values are presented as percentages stacked on the y-axis, where all values add up to 100%.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/e085dae5dd6aec8779a3b86754655b91251ec655/images/New_version5/TD_Visu_Image4.png)
<b><font color = "Black"> Image 4</b>

## Pie Chart 

Pie Chart are divided into slices to illustrate numerical proportions of the data.

 <b>3.</b>  Choose chart type <b>PIE</b> from given drop-down list compare the data using Pie chart.
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/342ffdef70f63d84c311d6a89e8697fc0b4f932b/images/New_version5/TD_Visu_Image5.png)
**Image 5**

### Editing Options for Pie Chart
 
- **Show percentage**  on selecting this checkbox, it displays percentage value for each measure in pie chart. if disabled it  displays dimension name. 

- **Polar Area** On selecting polar area check box it enables polar view for each dimensions field in a pie chart.
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/79a4c25fef2c47376b4eb788dd65249da7297afa/images/New_version5/TD_Visu_Image6.png)
**Image 6**

-  **Donut** donut chart are equal to pie chart. They show relationships of parts to a whole. select **Check Box** to enables the donut view.
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/79a4c25fef2c47376b4eb788dd65249da7297afa/images/New_version5/TD_Visu_Image7.png)
**Image 7**

## Radar chart 

 Radar charts are great way to compare members of a dimension in a function of several metrics.  
**For example:** when you want to buy a Laptop, you can use a radar chart to compare several devices across several metrics like battery life, memory, hard drive etc.  

 **4.** Choose chart type **RADAR** from given drop-down list compare the data using Radar chart.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/7482c4048b2b436faf52562e46d69819e6ac9484/images/New_version5/TD_Visu_Image10.png)
**Image 8**

- **Points (General)** on selecting the checkbox it enables pointers for the data range in line chart.

- **Point style(General)** will specify how the data points will appear on chart.
 Below are the following point styles available in AcuBi.  
  - Circle
  - Triangle
  - Rectangle
  - RectRot
  - Cross
  - CrossRot
  - Star
  - Line
  - Dash
  
- **Reverse scale**  it displays the inverse values.
**For Instance :** if the chart displays the 10 highest values, on Checking Reverse Scale , it displays 10 lowest values.

- **Show ticklabels** it enables measure values on y-axis.

- **Show arc lines** it points the dimension fields in radar chart.

- **Arc field** select the dimension field to apply arc lines.

- **Curve** it maximum and minimize the surface area in radar chart.

## Widget chart 

It displays one or more data series as a data graph. Widget chart is used to display the number of records created today. number of Incidents by status or department.

 **5.** Choose chart type **Widget** from drop-down list to compare the data using widget chart.
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/d5097c9535f891900b489566548ee000d4ae5204/images/New_version5/TD_Visu_Image8.png)
**Image 9**

- **Value** select the measure to show in the widget. you can use this field to specify the measure field if you have multiple measure value defined in the underlying step.

- **Format** select the number format for the measure field.

- **Previous value** select the second measure value for widget.

- **Change** specify the conditions for selected measures such as difference, growth, none.

- **Show growth** displays the growth rate of selected measures.

- **Title** specify widget title.

- **Label** specify the widget label.

- **Style** specify a status indicator for measure value such as default, primary, success, warning, info, danger.

##  World chart 

 It displays the data grouped by specific country and at the same time the grouped data regions are highlighted in the map.
 
**6.** Choose chart type **World** from drop-down list to compare the data using world chart.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/330a0df31c356ab5fcfde28fddd009f959e5f10d/images/New_version5/TD_Visu_Image23.png)
 **Image 10**
 
 > **Note :** The values you want to define in world chart, should be defined in model section. On defining in model the data field values will be displayed here.  
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/330a0df31c356ab5fcfde28fddd009f959e5f10d/images/New_version5/TD_Visu_Image24.png)
 
 **Image 11**
 
- **Title** specify a title for world map.

- **Flat Map** displays a flat view or "2D" vision of the map.

- **Default** set default colour to display specific countries.

- **Over Border** colour the border of a map region.

- **Data Field** choose the data field to display it on map.	

- **Tip Fields** select numbers of data fields to be displayed on map.
- **Colour Field** specifies which field to be colored.

- **Colour From & To** specify the color specific range of values in map region.

- **Negative Cutoff** enabled when negatives values are applicable.

- **Negative colour-from & to** Specify colour for specific range of negative values.

## Bar Chart

Bar charts are used to compare data across different categories. You can build a bar chart by placing a dimension on the X-axis and a measure on the Y-axis.

 **7.** .Choose chart type **BAR** from given drop-down list compare the data using Bar chart.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/94ba4dbdd16bfef4193c756dfae1a0dbef16d9fb/images/New_version5/TD_Visu_Image11.png)
**Image 12**

## Bubble chart 

It is used to display the data in circles. We can define each bubble using Dimension value and size by Measure value.
 
 **8.** .Choose chart type **BUBBLE** from given drop-down list compare the data.
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/91b2a584b941b19f94d1c93e5a856b8de3ebe51c/images/New_version5/TD_Visu_Image12.png)
**Image 13**

## Table chart 
 
Table chart displays the data in series making it more feasible for comparing dimensions and measure values.
 
 **9.** Choose chart type **Table** from drop-down list.
  ![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/08c494f9fa806d23afe1ace4e408a1f94d08d824/images/New_version5/TD_visu_image13.png)
**Image 14**

### Hide Pivot

To hide the first or last column field values in Visualization, Select hide first or hide last check box in Data section.
To carry out this function you need to derive a expression in calculated column.

**For Example** : Apply subtraction for Quantity_Sum and derive the expression in calculated column as follow;

```
pivot_offset(#{biplus.orders.sum_quantity},0,-1)
```

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b297a288ba4fa4e9db7a19c43c2f2751ad0f1130/images/New_version5/TD_Visu_Image14.png)
**Image 15**

The resultant for this expression would be seen in green color;

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b08a20448157551a2870e258c70ea7f81adf4b1d/images/New_version5/TD_Visu_Image15.png)
**Image 16**

In the above image you can see, hide_pivot 1st column is seen empty, so in order to hide this you need to select checkbox **pivot hide first** in **Data Section** to hide it in visualization charts. ( Applicable only for table chart). 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/9364e4dc946533da5edb31847a634646c86b3ae5/images/New_version5/TD_Visu_Image16.png)
**Image 17**

Similarly, to hide last column, select check_bob Hide_Last.

## Funnel chart 

Funnels helps to visualize a process that has stages and items flow sequentially from one stage to the next. Use a funnel when there is a sequential flow between stages, such as a sales process that starts with inquiry and ends with billing.

**The following section describes the editing option for bubble chart in visualization;**
 
 **10.** Choose chart type **Funnel** from drop down-list.
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/2f2fb255d5529d8fd300f252e2ce61aba3985755/images/New_version5/TD_Visu_Image17.png)
**Image 18**

**AcuBi** displays funnel charts in following formats:

 - **Sort:** it enables data in the sorted order in funnel chart.
 
 - **Curved:** it enables the curved view for funnel chart.
 
- **Pinched:** :enable compressed view of funnel chart

- **Inverted:**  enables inverted view of Funnel chart

- **Highlight on hover:** highlights on moving hover on funnel chart.

- **Dynamic Height:** Enables dynamic height for the measure field with maximum value.

- **Load Animation:** Enables animation view to funnel chart

##  Gauge Chart 

Gauge chart displays current status in the context of goal.

 
 **11.** Choose chart type **Guage** from drop-down list.

- **Green** colour in gauge chart indicates the value attained is closer to target.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b4838dece9a608f6372b8e6e1ad4c52a8955d4ec/images/New_version5/TD_Visu_Image18.png)
**Image 19**

- **Orange** colour indicates the maximum value attained is half the way to target and **Red** colour indicates the maximum value attained is at initial state or lower side of the target. 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/master/images/New_version5/TD_Visu_Image19.png)
**Image 20**

- **Value** select one of the available measure values from the drop down.

- **Min** specifies the minimum value of the gauge this corresponds to bottom position of the gauge.

- **Max**  specifies the maximum value of the gauge this corresponds to top position of the gauge.

- **Title** specify a title.

- **Label** specify a identifier name to display in the chart.

- **Donut** displays total measure value.

- **Counter** displays minimum and maximum values of the measure.

- **Reverse** displays the measure values in reversal direction maximum to minimum.

- **Hide Minmax**  hides min and maximum values in gauge target.



# Standard Editing Option in Charts

## General Section 

- **Title** specify title for the chart selected.

- **Position** align title to top,bottom,left,right position.

- **Label** Specify label text.

- **Padding** specifies spacing at the top,bottom,left and right side of the charts and Axis. it accepts the number range in between 0 to 100.

- **Tooltips** if the underlying field defines a description for a measure, that description is displayed on moving the hover over the column.

- **Grouped Tooltips** if more than one measure field is selected, it displays both the measure values on moving the hover over the column.

- **Show legend** on selecting the checkbox it displays the measures fields used at the bottom of the chart, you can display or hide specific measure field values on chart by clicking on the measure field.

- **Position** Align the legend at top,bottom,left and right side of the chart.

- **Include Nulls** on selecting this checkbox it displays **Null Values** retrieved in Charts section.

- **Display Labels** on selecting this checkbox, it displays the data value obtained for the fields.

- **Background Enabled**  it enables background colour for labels.

- **Font Weight**  Set the label font to normal ( default) or Bold text.

- **Font Size** Enable font size for label.

- **Border radius** Set the label border radius to a given range.

- **Rotation** This option controls the clockwise rotation angle (in degrees) of the label, the rotation center point being the label center. The default value is 0 (no rotation).

-  **Align**   it defines the position of the label relative to the anchor point position and direction. Its value can be expressed by one of the following string presets:

   -   **Start** the label is positioned before the anchor point, following the same direction
   -   **End** the label is positioned after the anchor point, following the same direction
   -   **Center (default)** the label is centered on the anchor point
   -   **Right** the label is positioned to the right of the anchor point (0°)
   -   **Bottom** the label is positioned to the bottom of the anchor point (90°)
      -   **Left** the label is positioned to the left of the anchor point (180°)
   -   **Top** the label is positioned to the top of the anchor point (270°)
  - **Anchor** The label position is calculated based on the anchor option. AcuBi supports Following positioning.

    -   **Center  (default)** aligns the Label in center.
    -   **Start** aligns the the label at lowest boundary.
    -   **End** aligns the label at highest boundary.
    
- **Align Negative** It will enable the negative values to be displayed below range  `0`.
 
 ## Data 

- **Row Grouping** displays the grouped value of the duplicate fields.

- **Explore Enabled** on selecting the checkbox, it allows you to view the  data which has been grouped or else it displays only the consolidated value.

- **Legend** displays the measure.

- **Format** Choose the number format for measure value.

- **Currency**  Cheese the currency format for  measure value.

- **Y Axis** Choose the measure values to be displayed on chart.

- **Column Aggregate ( Table View)** Type of aggregate value to be displayed for a measure.

- **Custom Tooltip** on moving the hover on the column it displays the customized new value. 

> **Example** : in case if we are taking two measures than you can interchange the measure fields values on the column as per the requirement. 

- **Custom Label** Using this option you can display your own label for the column field values. 
##{start: }#{sum_rate} as of #{sum_amount}##{end: }

- **Bubble Size( Bubble Chart)** Depending on measure values, it varies in size.
 
## X-Axis 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/1199f45790ebb995f76c92d0d25a8beacade92cf/images/New_version5/TD_Visu_Image21.png)
**Image 21**

- **Axis type** specifies the how x-axis scale for Line, Bar,Bubble is calculated and displayed.

  - **Indexed** specifies the data to be plotted in numeric values starting from zero on x-axis.
   
  - **Category** specifies the data to be plotted as category group on x-axis.
  
  - **Timeseries** specify the data to be plotted as time values. The x-axis is labeled with appropriate time increments.
 
-  **X-Grid Color** display specific color on X-axis.

- **X-Axis Font Color** Enables different color option for the values on X-axis.

- **X-Axis**  specify a dimension or a measure( Horizontal Bar) field on X-axis.

- **Show Grid** enables the grid display for dimension fields on x-axis.

- **Axis label** Label text  for x-axis.

**Reference Lines** enables the creation of reference lines in a chart.

 - **Reference** specify a indicator name. 
  
 - **Type** specify reference type as line or  area.
  
 -  **From & to** specify the reference line for specific range of dimensions.

 - **Theme** enables colour for reference line.
 
 > **Note:**  X-Axis is enabled only for Line, Bar and Bubble chart only.

## Y-Axis

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/1199f45790ebb995f76c92d0d25a8beacade92cf/images/New_version5/TD_Visu_Image22.png)
**Image 22**

- **Axis** select the measures values on y-axis  to enable
editing options for y-axis in Line, Bar and bubble chart.

- **Axis label** Text label for x-axis.

- **Format** it enables number format for numeric values.

-  **Y-Grid Color** display different color on Y-axis.

- **Y-Axis Font Color** Enables different colors for the dimensions ( Horizontal Bar) or Measures on Y-axis.

- **Y-Axis** display dimensions or measures ( Horizontal bar) values on Y-axis. 

- **Show Grid** enables the grid display on y-axis.

- **Include Zero** displays measure values starting from zero.

- **Position** you can can align the y-axis to left or right side of the chart.

**Reference Lines** enables the creation of reference lines in a chart.

- **Name** specify a reference name for specific information on y-axis.
  
 - **Type** specify  Linear, Polynomial, Exponential, Logarithmic, Average, Median, Minimum, Maximum, Deviation, Variance, Custom Line, Custom Area on Y-axis.
  
 -  **From & to** specify the reference line for specific range of measure values.

 - **Theme** enables colour for reference line.
 
 > **Note:**  Y-Axis is enabled only for Line, Bar and Bubble chart only.
 
## Format   
      
- **Condition** Specify any of the following condition types Greater than, Less than, Between, Not Between, equal to, duplicates values, Top 10 Items, Bottom 10 Items, Above Average, Below Average for the fields.

- **Format on** Specify a measure field on which you want to apply format.

- **Value** Specify a value to measure the condition.

- **BG (background colour)** Select the background colour for the data which is retrieved using condition.

- **Font** Select the font colour for the data retrieved based on condition.

- **Icon** Select a icon for the data retrieved based on condition.

- **Before number** Align the icon before or after the data.


**For Example :** Consider below image, which displays the format section for table chart.


![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/1199f45790ebb995f76c92d0d25a8beacade92cf/images/New_version5/TD_Visu_Image20.png)
**Image 23**

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE2NjAzMzY5MzEsLTcxNjMzNjk3NiwtOD
Q0Njg5MzQ4LDE4NDMwNTcyNjEsOTI0NzEyOTE0LC0xMTQzMjc4
Njc4LDQ5OTM4ODIyLC0yMDE5ODEwNDcwLDEwMzYzNjgxNTcsLT
EyODIwNDM2NTksLTExNTM1MTAwNDEsMjc4ODI0MTgyLDgyMjkz
OTkzOSwtMTQ2ODA3NDc2LC0xODQzODI5MjM4LC03MzU3ODM3Mz
gsNDc3NTU2MTk5LDMyNTcwNTU4OSw3NTEwOTM5NCwtMTUzMjkx
MDEwOV19
-->