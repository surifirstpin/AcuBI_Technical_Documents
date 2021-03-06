


<center><h1>Visualization Charts</h1></center>


<b>AcuBi</b> has an ability to create graphics and charts based on the result obtained in reports section. Charts displays different type of pictorial representation of the data.  AcuBi keeps query details and visualization(Charts) configuration data together, so user can see data and visualization charts together when it is shared to them.


## Getting Started With Visualization

Let us see in details how to configure visualization. Click on <b>Charts</b> tab to configure visualization option for the result obtained. 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/52de5df82ef6986d3c2224728e8100490c41ad22/images/New_version5/TD_Visu_Image1.png)
<b><font color = "Black"> Image 1</b>


## Types of Visualization

AcuBi visualization charts are used based on the priority of what specific information you want to view about the data retrieved. Each type of  chart has different customization option for its appearance. It provides an ability to visualize the data in 11 different types of charts with some standard editing options. 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/0dc367172608197f5a129c93f4c0c2992c7bb50c/images/New_version5/TD_Visu_Image2.png)
<b><font color = "Black"> Image 2</b>

#### List of chart types 
 - <b>Line</b>
 - <b>Horizontal Bar</b>
 - <b>Pie</b>
 - <b>Radar</b>
 - <b>Widget</b>
 - <b>Bar</b>
 - <b>Bubble</b>
 - <b>Table </b>
 - <b>Funnel</b>
 - <b>World</b>

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
  
- <b>Points</b>  will display the data by specifying pointers on chart.

- <b>Point style</b> will specify how the data pointers will appear on chart. 

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

Horizontal Bar charts are used to compare data across different categories horizontally. You can build a bar chart by placing a dimension on Y-axis and a measure on X-axis.

 <b>2.</b> Choose chart type <b>HORIZONTAL BAR</b> from drop-down list to compare the data using horizontal chart.
 
- <b>Stacked (Data)</b> Series of values are added on the Y-axis by displaying each consecutive values above the last. 

- <b>100% Stacked (Data)</b>  Series of values are presented as percentages stacked on the y-axis, where all values add up to 100%.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/e085dae5dd6aec8779a3b86754655b91251ec655/images/New_version5/TD_Visu_Image4.png)
<b><font color = "Black"> Image 4</b>

## Pie Chart 

Pie Chart are divided into slices to illustrate numerical proportions of the data.

 <b>3.</b>  Choose chart type <b>PIE</b> from drop-down list compare the data using Pie chart.
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/342ffdef70f63d84c311d6a89e8697fc0b4f932b/images/New_version5/TD_Visu_Image5.png)
<b><font color = "Black"> Image 5</b>

### Editing Options for Pie Chart
 
- <b>Show percentage</b>  on selecting this checkbox, it displays percentage value for each measure in pie chart. if disabled it displays dimension name. 

- <b>Polar Area</b> On enabling polar area it displays polar region of each dimensions field in a pie chart.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/79a4c25fef2c47376b4eb788dd65249da7297afa/images/New_version5/TD_Visu_Image6.png)
<b><font color = "Black"> Image 6</b>

-   **Show value** on enabling this checkbox, it displays value for each measure in pie chart. If disabled it displays dimension name.

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/P1.png?raw=true)
<b><font color = "Black"> Image 7</b>
  

-   **Value & Percent** on selecting this checkbox, it displays value and percentage value for each measure in pie chart. If disabled it displays dimension name.


![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/P2.png?raw=true)
<b><font color = "Black"> Image 8</b>







-  <b>Donut</b> donut chart are equal to pie chart. They show relationships of parts to a whole. To enable this, choose <b>Check Box</b> for donut view.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/79a4c25fef2c47376b4eb788dd65249da7297afa/images/New_version5/TD_Visu_Image7.png)
<b><font color = "Black"> Image 9</b>

## Radar chart 

 Radar charts are great way to compare members of a dimension in a function of several metrics.  
<b>For example</b> when you want to buy a Laptop, you can use a radar chart to compare several devices across several metrics like battery life, memory, hard drive etc.  

 <b>4.</b> Choose chart type <b>RADAR</b> from given drop-down list compare the data using Radar chart.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/7482c4048b2b436faf52562e46d69819e6ac9484/images/New_version5/TD_Visu_Image10.png)
<b><font color = "Black"> Image 10</b>

- <b>Points (General)</b> on selecting the checkbox it enables pointers for the data range in line chart.

- <b>Point style(General)</b> will specify how the data points will appear on chart.

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
  
- <b>Reverse scale</b>  it displays the inverse values.

<b>For Instance </b> if the chart displays the 10 highest values, on Checking Reverse Scale , it displays 10 lowest values.

- <b>Show Tick-labels</b> it enables measure values on y-axis.

- <b>Show arc lines</b> it points the dimension fields in radar chart.

- <b>Arc field</b> select the dimension field to apply arc lines.

- <b>Curve</b> it maximize and minimize the surface area in radar chart.

## Widget chart 

It displays one or more data series as a data graph. Widget chart is used to display the number of records created today. number of Incidents by status or department.

 <b>5.</b> Choose chart type <b>Widget</b> from drop-down list to compare the data using widget chart.
 
 ![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/Widget1.png?raw=true)
<b><font color = "Black"> Image 11</b>

**Value** select the measure to show in the widget. you can use this field to specify the measure field if you have multiple measure value defined in the underlying step

 - <b>Field Type</b> select the field type measure or dimension.

- <b>Value</b> select value for first measure field.
- <b>Format</b> select the number format for the measure field.

- <b>Previous value</b> select the second measure value for widget.

- <b>Change</b> specify the conditions for selected measures such as difference, growth, none.

- <b>Show growth</b> displays the growth rate of selected measures.

- <b>Title</b> specify widget title.

- <b>Label</b> specify the widget label.

- <b>Style</b> specify a status indicator for measure value such as default, primary, success, warning, info, danger.

- <b>Theme</b> Select the suitable theme for widget chart.

- <b>Widget Icon</b> Select suitable icon for widget values.


- <b>BG Colour</b> Select back ground color for widget chart.

##  World chart 

 It displays the data grouped by specific country and at the same time the grouped data regions are highlighted in the map.
 
 > <b>Note :</b> The values you want to define in world chart, should be defined in model section. On defining in model the data field values will be displayed here.  

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/330a0df31c356ab5fcfde28fddd009f959e5f10d/images/New_version5/TD_Visu_Image24.png)
 <b><font color = "Black"> Image 12</b>

<b>6.</b> Choose chart type <b>World</b> from drop-down list to compare the data using world chart.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/330a0df31c356ab5fcfde28fddd009f959e5f10d/images/New_version5/TD_Visu_Image23.png)
<b><font color = "Black"> Image 13</b>
 

- <b>Title</b> specify a title for world map.

- <b>Flat Map</b> displays a flat view or "2D" vision of the map.

- <b>Default</b> set default color to display specific countries.

- <b>Over Border</b> color the border of a map region.

- <b>Data Field</b> choose the data field to display it on map.	

- <b>Tip Fields</b> select numbers of data fields to be displayed on map.

- <b>Color Field</b> specifies which field to be colored.

- <b>Color From & To</b> specify the color specific range of values in map region.

- <b>Negative Cutoff</b> enabled when negatives values are applicable.

- <b>Negative color-from & to</b> Specify color for specific range of negative values.

## Bar Chart

Bar charts are used to compare data across different categories.hi You can build a bar chart by placing a dimension on the X-axis and a measure on the Y-axis.

 <b>7.</b>Choose chart type <b>BAR</b> from given drop-down list compare the data using Bar chart.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/94ba4dbdd16bfef4193c756dfae1a0dbef16d9fb/images/New_version5/TD_Visu_Image11.png)
<b><font color = "Black"> Image 14</b>

## Bubble chart 

It is used to display the data in circles. We can define each bubble using dimension value and size by measure value.
 
 <b>8.</b> Choose chart type <b>BUBBLE</b> from given drop-down list compare the data.
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/91b2a584b941b19f94d1c93e5a856b8de3ebe51c/images/New_version5/TD_Visu_Image12.png)
<b><font color = "Black"> Image 15</b>

## Table chart 
 
Table chart displays the data in series making it more feasible for comparing dimensions and measure values.
 
 <b>9.</b> Choose chart type <b>Table</b> from drop-down list.
  ![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/Table1.png?raw=true)
<b><font color = "Black"> Image 16</b>

-   Now click on  Bets EUR in Datasets

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/Table%202.png?raw=true)
<b><font color = "Black"> Image 17</b>


-   **Header Color** displays the color which is choosed in drop down.
    

  

-   **Hfont-weight** enables the font size of the header
    

  

-   **Footer-FontWeight** enables the font size of the footer
    

  

-   **Format** choose the number format for measure value.
    

  

-   **Currency** choose the currency format for measure value.
    

  

  

-   **Column Agg** Type of aggregate value to be displayed for a measure.

## Header Flipping

 Header Flipping which is applied to dimension field and for Table chart view.

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/H1.png?raw=true)
<b><font color = "Black"> Image 18</b>

-   Select Format Column in dropdown list and that is displayed in the header as shown in below image.

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/H2.png?raw=true)
<b><font color = "Black"> Image 19</b>

**Note:** Header Flipping in not applicable for any chart except Table chart.

-   It is reflected the same in the dashboard.

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/H3.png?raw=true)
<b><font color = "Black"> Image 20</b>


### Hide Pivot (Hide first, Hide last)

To hide the first or last column field values in Visualization Table, Select hide first or hide last check box in Data section.
To carry out this function you need to derive a expression in calculated column.

<b>For Example</b> : Apply subtraction for Quantity_Sum and derive the expression in calculated column as follow;

```
pivot_offset(#{biplus.orders.sum_quantity},0,-1)
```

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b297a288ba4fa4e9db7a19c43c2f2751ad0f1130/images/New_version5/TD_Visu_Image14.png)
<b><font color = "Black"> Image 21</b>

The resultant for this expression would be seen in green color;

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b08a20448157551a2870e258c70ea7f81adf4b1d/images/New_version5/TD_Visu_Image15.png)
<b><font color = "Black"> Image 22</b>

In the above image you can see, hide_pivot 1st column is seen empty, so in order to hide this you need to select checkbox <b>pivot hide first</b> in <b>Data Section</b> to hide it in visualization charts. (Applicable only for table chart). 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/9364e4dc946533da5edb31847a634646c86b3ae5/images/New_version5/TD_Visu_Image16.png)
<b><font color = "Black"> Image 23</b>

Similarly, to hide last column, select check_bob Hide_Last.

## Funnel chart 

Funnels helps to visualize a process that has stages and items flow sequentially from one stage to the next. Use a funnel when there is a sequential flow between stages, such as a sales process that starts with inquiry and ends with billing.

<b><i>The following section describes the editing option for bubble chart in visualization;</i></b>
 
 <b>10.</b> Choose chart type <b>Funnel</b> from drop down-list.
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/2f2fb255d5529d8fd300f252e2ce61aba3985755/images/New_version5/TD_Visu_Image17.png)
<b><font color = "Black"> Image 24</b>

<b><i> You can view the funnel charts in following formats by enabling checkbox for below mentioned fields;</i></b>

 - <b>Sort</b> it enables data in the sorted order in funnel chart.
 
 - <b>Curved</b> it enables the curved view for funnel chart.
 
- <b>Pinched</b> enable compressed view of funnel chart

- <b>Inverted</b>  enables inverted view of Funnel chart

- <b>Highlight on hover</b> highlights on moving hover on funnel chart.

- <b>Dynamic Height</b> Enables dynamic height for the measure field with maximum value.

- <b>Load Animation</b> Enables animation view to funnel chart

##  Gauge Chart 

Gauge chart displays current status in the context of goal.

 
 <b>11.</b> Choose chart type <b>Guage</b> from drop-down list.

- <b>Green</b> color in gauge chart indicates the value attained is closer to target.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b4838dece9a608f6372b8e6e1ad4c52a8955d4ec/images/New_version5/TD_Visu_Image18.png)
<b><font color = "Black"> Image 25</b>

- <b>Orange</b> color indicates the maximum value attained is half the way to target and <b>Red</b> color indicates the maximum value attained is at initial state or lower side of the target. 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/master/images/New_version5/TD_Visu_Image19.png)
<b><font color = "Black"> Image 26</b>

- <b>Value</b> select one of the available measure values from the drop down.

- <b>Minimum</b> specifies the minimum value of the gauge this corresponds to bottom position of the gauge.

- <b>Maximum</b>  specifies the maximum value of the gauge this corresponds to top position of the gauge.

- <b>Title</b> specify a title.

- <b>Label</b> specify a identifier name to display in the chart.

- <b>Donut</b> displays total measure value.

- <b>Counter:</b> displays minimum and maximum values of the measure.

- <b>Reverse</b> displays the measure values in reversal direction maximum to minimum.

- <b>Hide Minmax</b>  hides min and maximum values in gauge target.


# Fine Tuning Visualization Charts

## General Section 


- <b>Title</b> specify title for the chart selected.

- <b>Position</b> align title to top, bottom, left, right position.

- <b>Label</b> Specify label text.

- <b>Padding</b> Specifies spacing at the top, bottom, left and right side of the charts and axis. It accepts the number range in between 0 to 100.

- <b>Tooltips</b> if the underlying field defines a description for a measure, that description is displayed on moving the hover over the column.

  - <b>Tooltip Background</b> Enables background color for underlying field info.
 
  - <b>Tooltip Color</b> Enable color for field information displayed.
  
  - <b>Title Color</b>  Enables color for field.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/f6b12c66e409436d4be04517aaa3b98f09dc668f/images/New_version5/td_visu4.png)

<b><font color = "Black"> Image 27</b>

- <b>Grouped Tooltips</b> if more than one measure field is selected, it displays both the measure values on moving the hover over the column.

- <b>Show legend</b> on selecting the checkbox it displays the measures fields used at the bottom of the chart, you can display or hide specific measure field values on chart by clicking on the measure field.

- <b>Position</b> Align the legend at top,bottom,left and right side of the chart.

- <b>Include Nulls</b> on selecting this checkbox it displays <b>Null Values</b> retrieved in Charts section.

- <b>Display Labels</b> on selecting this checkbox, it displays the data value obtained for the fields.

- <b>Background Enabled</b>  it enables background colour for labels.

- <b>Font Weight</b>  Set the label font to normal ( default) or Bold text.

- <b>Font Size</b> Enable font size for label.

- <b>Border radius</b> Set the label border radius to a given range.

- <b>Rotation</b> This option controls the clockwise rotation angle (in degrees) of the label, the rotation center point being the label center. The default value is 0 (no rotation).

-  <b>Align</b>   it defines the position of the label relative to the anchor point position and direction. Its value can be expressed by one of the following string presets:

   -   <b>Start</b> the label is positioned before the anchor point, following the same direction
   -   <b>End</b> the label is positioned after the anchor point, following the same direction
   -   <b>Center (default)</b> the label is centered on the anchor point
   -   <b>Right</b> the label is positioned to the right of the anchor point (0°)
   -   <b>Bottom </b>the label is positioned to the bottom of the anchor point (90°)
   -   <b>Left</b> the label is positioned to the left of the anchor point (180°)
   -   <b>Top</b> the label is positioned to the top of the anchor point (270°)

- <b>Anchor</b> The label position is calculated based on the anchor option. AcuBi supports Following positioning.

   -   <b>Center  (default)</b> aligns the Label in center.
   -   <b>Start</b> aligns the the label at lowest boundary.
   -   <b>End</b> aligns the label at highest boundary.
    
- <b>Align Negative</b> It will enable the negative values to be displayed below range  `0`.
 
## Data

- <b>Row Grouping </b> displays the grouped value of the duplicate fields.

- <b>Explore Enabled </b> on selecting the checkbox, it allows you to view the  data which has been grouped or else it displays only the consolidated value.

- <b>Legend </b> displays the measure.

- <b>Format </b> Choose the number format for measure value.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/441779bb16723c8362f3319094f99be96a250594/images/New_version5/Td_Visu1.png)

- <b>Currency </b>  Cheese the currency format for  measure value.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/441779bb16723c8362f3319094f99be96a250594/images/New_version5/td_visu3.png)

- <b>Y Axis </b> Choose the measure values to be displayed on chart.

- <b>Column Aggregate ( Table View) :</b> Type of aggregate value to be displayed for a measure.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/441779bb16723c8362f3319094f99be96a250594/images/New_version5/td_visu2.png)


- <b>Custom Tooltips </b> on moving the hover on the column it displays the customized new value. 

> <b>Example</b> : in case if we are taking two measures than you can interchange the measure fields values on the column as per the requirement. 

- <b>Custom Label </b> Using this option you can display your own label for the column field values. 
##{start: }#{sum_rate} as of #{sum_amount}##{end: }

- <b> Render Label  </b> Make underlying measure value available or visible.

- <b>Bubble Size (Bubble Chart)</b> Depending on measure values, it varies in size.

 ![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/05951e453ff2bcd8b3afd29f0b02b488113e0025/images/New_version5/td_visu_image28.png)

<b><font color = "Black"> Image 28</b>

## X-Axis 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/1199f45790ebb995f76c92d0d25a8beacade92cf/images/New_version5/TD_Visu_Image21.png)
<b><font color = "Black"> Image 29</b>

- <b>Axis type </b> specifies the how x-axis scale for Line, Bar,Bubble is calculated and displayed.

  - <b>Indexed </b> specifies the data to be plotted in numeric values starting from zero on x-axis.
   
  - <b>Category </b> specifies the data to be plotted as category group on x-axis.
  
  - <b>Timeseries : </b> specify the data to be plotted as time values. The x-axis is labeled with appropriate time increments.
 
-  <b>X-Grid Color</b> display specific color on X-axis.

- <b>X-Axis Font Color </b> Enables different color option for the values on X-axis.

- <b>X-Axis </b>  specify a dimension or a measure( Horizontal Bar) field on X-axis.

- <b>Show Grid </b> enables the grid display for dimension fields on x-axis.

- <b>Axis label </b> Label text  for x-axis.

- <b>Reference Lines </b> enables the creation of reference lines in a chart.

 - <b>Reference </b> specify a indicator name. 
  
 - <b>Type </b> specify reference type as line or  area.
  
 -  <b>From & to </b> specify the reference line for specific range of dimensions.

 - <b>Theme </b> enables color for reference line.
 
 > <b>Note </b>  X-Axis is enabled only for Line, Bar and Bubble chart only.

## Y-Axis

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b6c2628d58b42d23d022e28b9b3bee1c44a10e73/images/New_version5/TD_Visu_Image22.png)

<b><font color = "Black"> Image 30</b>

- <b>Axis  </b> select the measures values on y-axis  to enable
editing options for y-axis in Line, Bar and bubble chart.

- <b>Axis label </b> Text label for x-axis.

- <b>Format </b> it enables number format for numeric values.

-  <b>Y-Grid Color  </b> display different color on Y-axis.

- <b>Y-Axis Font Color </b> Enables different colors for the dimensions ( Horizontal Bar) or Measures on Y-axis.

- <b>Y-Axis  </b> display dimensions or measures ( Horizontal bar) values on Y-axis. 

- <b>Show Grid </b> enables the grid display on y-axis.

- <b>Include Zero </b> displays measure values starting from zero.

- <b>Position </b>  align y-axis to left or right side of the chart.

- <b> Min Value</b>  Displays Y-axis data starting from value specified in field <b>Min Value</b>

#### Reference Lines

<b>Reference Lines : </b> enables the creation of reference lines in a chart.

- <b>Name </b> specify a reference name for specific information on y-axis.
  
- <b>Type : </b> specify  Linear, Polynomial, Exponential, Logarithmic, Average, Median, Minimum, Maximum, Deviation, Variance, Custom Line, Custom Area on Y-axis.
  
-  <b>From & to </b> specify the reference line for specific range of measure values.

- <b>Theme </b> enables color for reference line.
 
  
 
 1.Click on Add Reference Line.

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/Ref1.png?raw=true)
<b><font color = "Black"> Image 31</b>

<b>Note:</b> Y-Axis is enabled only for Line, Bar and Bubble chart only.

 2.  Showing the **Reference Line 1** by selecting the Data Field (Bets Euro) for Type (Linear)

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/Ref2.png?raw=true)
<b><font color = "Black"> Image 32</b>

 3. Showing the **Reference Line 2** by selecting the Data Field (Wins Euro) for Type (Polynomial)
 
![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/Ref3.png?raw=true)
<b><font color = "Black"> Image 33</b>


 4. Showing the **Reference Line 3** by selecting the Data Field (Total) for Type (Exponential)

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/Ref4.png?raw=true)
<b><font color = "Black"> Image 34</b>

 
# Format   
      
 Format arranges a pattern for information which is stored in database.

> Note:  Consider below image, which displays the format section for table chart.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/1199f45790ebb995f76c92d0d25a8beacade92cf/images/New_version5/TD_Visu_Image20.png)
<b><font color = "Black"> Image 35</b>

- <b>Condition : </b> Specify any of the following condition types  
   - Greater than
   - Less than
   - Between
   - Not Between
   - Equal to, duplicates values
   - Top 10 Items
   - Bottom 10 Items
   - Above Average
   - Below Average

- <b>Format on </b> Specify a measure field on which you want to apply format.

- <b>Value </b> Specify a value to measure the condition.

- <b>BG (background color) </b> Select the background color for the data which is retrieved using condition.

- <b>Font </b> Select the font color for the data retrieved based on condition applied.
   
   - Choose a color using drop down menu.

   ![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b84cdf8d077562656baf6f5c2d08d36c54abc760/images/New_version5/TD_Visu_Image25.png)
  
   
# Custom Color

To create Custom color, First click on <b> Custom Color</b>. Use the color picker to choose the colour. 

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b84cdf8d077562656baf6f5c2d08d36c54abc760/images/New_version5/TD_Visu_Image26.png)
 


You can either change the color by placing <b>hexstring</b> such as <b>#6d9ac7,</b> or color name, such as darkblue into the color value box at the bottom of the picker.

  ![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/180ee79d0c233ce60042245d66c6a69bbed52fe2/images/New_version5/TD_Visu_Image27.png)


- <b>Icon</B> Select a icon for the data retrieved based on condition.

- <b>Before number</b> Align the icon before or after the data.



<!--stackedit_data:
eyJoaXN0b3J5IjpbMTM3NzU5Njk4OCwtMTg0NTYwNjMxOCw3Mz
Q3Mjk5NzQsMTQzNjk5MTE1MCw3NDQ1NTU1NzcsLTE4NTQ3OTg2
MTEsLTEyMTA1NDAwNTQsLTE5NDIzNTAxNTEsLTkzNzUyODI3My
wtMjIwMzk1MDM1LC0xNDk2OTMxMTU1LC02ODg0NzgzNzIsMTgy
NjMxNTA5NSwyNTMzODk1OTQsMTMyMzY3NDA1NywxMjgzNDQzND
g3LDY2MDQ4MTE3NiwtMTAzMjAzNTE5NCwtMTU2MDEzNDU1NCwt
NDI1MDI1OTc2XX0=
-->