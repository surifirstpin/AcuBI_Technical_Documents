<h1><center>Overlay</center> </h1>

  

<b> Functionality :  </b> Overlay is implemented to bring the particular field from one table to the another table excluding joins with in the database.

  

-   overlay_dimensions ,overlay_table and field_type are the key factors which plays a vital role in the overlay functionality.
    

-   overlay fields which are measures only, will be retrieved based upon the combination of overlay dimensions retrieve
    

  

-   It is essential to use atleast one dimension field which are defined in overlay_dimensions
    

<b> Interpretation :  </b> During the time of proceeding using joins makes the database server has to do more work, which means that it is more time consuming process to retrieve data. In this objective we can use overlay to fetch the particular field from one table to the another table.

  
<b> Navigation :  </b> Go to Model section firstly, we need to define the overlay fields as shown below:

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/O1.png?raw=true)
<b><font color = "Black" >Image1 </font></b>

  

-   Operate to **Reports** section and select the desired project and Model based on the field which is mentioned in the overlay dimensions

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/O2.png?raw=true)
 <b><font color = "Black" >Image 2 </font></b>

-   In case take dimension field which is not mentioned in overlay dimension as shown below it gives no data.
![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/O3.png?raw=true)
<b><font color = "Black" >Image 3</font></b>


**Overlay Dimensions Rules:**

  

1. Format for overlay_table_column_name need to mention as destination_table_column_name

  

  

  

  

2. For report While selecting the field (Dimension only) , need to mention the alias name from destination table (Alias name will get from SQL tab after selecting the field) as shown in **Image 3.**













![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/O4.png?raw=true)
<b><font color = "Black" >Image 4 </font></b>



**Lets see in detail using a query :**

  

a. Take the sql from the report section that is image 4. and give the alias name as a

  

(SELECT

game_kpi.partner AS partner,

(select distinct count(bs.ngr) as summary_NGR from pragmatic_staging.bi_summary bs) AS summary_NGR

FROM pragmatic_staging.game_kpi AS game_kpi

GROUP BY (game_kpi.partner))a

  

b. Now take the sql from model section mentioned in image1 and consider the alias name as b.

  

(select distinct partnerid as partner, count(bs.ngr) as summary_NGR from pragmatic_staging.bi_summary bs group by partnerid) b

  

c. Then join the two queries using left join and finally gives the output result.









![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/O5.png?raw=true)
<b><font color = "Black" >Image 5 </font></b>
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4NzA5MzM0NTEsMTYzNzg4NzIyMSwtMj
EwODgxNDYsLTEzODI0NjM0NTldfQ==
-->