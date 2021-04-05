


<h1><center>Jobs</center> </h1>

Jobs are used for scheduling tasks to run on the server. They are most commonly used for automating system maintenance or administration at a specified time and date. Jobs are scheduled task itself, which are useful to automate repetitive tasks.

<b> Functionalities </b>

-   Jobs can be set to run in time interval such as by minute, hour, month, year or any of these combinations.
    
-   You can run jobs as many times as desired.
    

<b> Interpretention </b>

Proceeding with jobs can run repetitive tasks or can be scheduled insted of manual process and we can run job manually or you can configure it to run according to a schedule or in response to alerts. By generating alerts we can automatically get notification to users through job.

## Getting Started 

Navigate to <b><i>SQL Runner Section</i></b>-->Jobs-->Click <b><i>Create Job</b></i>

![Image 1](https://raw.githubusercontent.com/sv18042016/fp1/master/images/New_version5/TD_JOBS_IMAGE1.png)
 <b><font color = "Black" >Image 1</font></b>
 
 Enter the following information in Create Job Window;
 
 - <b>Job Name:</b> Name identifier for Job

 - <b>Info:</b> Job description
 
 - <b>Task Name:</b> Name identifier for Task
 
 - <b>Task Info:</b> Task description
 
 - <b>Task Type:</b> Select task type using drop down list.

![Image 2](https://raw.githubusercontent.com/sv18042016/fp1/23513febf6e72c734c80e805c286346a21504fb4/images/New_version5/TD_JOBS_IMAGE2.png)

 <b><font color = "Black" >Image 2</font></b>
  
<b>For Instance:</b> in this document, i am creating a Job for task type-->Query Execute.

On selecting query execute, it display following functionalities;

- <b>Source Connection:</b> Select database source connection.

- <b>Query:</b> Enter your query.

- <b> Global Block:</b> On selecting the checkbox for global block, the global type condition is applied for multiple tasks available under existing Job.

- <b>Block Type:</b> Select block type using drop down to get specific range of data at time by avoiding data crashing. Following are list of block types applicable;

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/481fb4c764374cf58150ced0707d94392d9bc2c2/images/New_version5/TD_JOBS_IMAGE1.png)


- <b>Block From & To:</b>  Enter the start and the ending point of the data to be fetched.

- <b>Block Size:</b> Enter specific run time range.

- <b>Block Key From & To:</b> It works as reference name ( applicable in case of where conditions)

Click <b>Save,</b> to save Job created.


> <b>Note: </b> Block type is applicable only for Date fields.

All the saved jobs are visible under SQL Jobs list.

![Image 3](https://raw.githubusercontent.com/sv18042016/fp1/b679c7e6d82f09c9795d0fc4c32bbe7ef5430c8d/images/New_version5/TD_JOBS_IMAGE3.png)
 <b><font color = "Black" >Image 3</font></b>

## Multiple Task

Click on Task button to create multiple Task in Jobs.

## Schedule Job

</b>1.</b> Click <b>Gear</b> Icon available next to existing Job name and Navigate to <b><i>Schedule.</i></b>

![Image 4](https://raw.githubusercontent.com/sv18042016/fp1/47f6e0897c275693ef1c3b372f71f513751c8641/images/New_version5/TD_JOBS_IMAGE4.png)

 <b><font color = "Black" >Image 4</font></b>

Under Schedule Job Window, Enter Below details;

- <b>Start delay:</b> Enter time delay to run the file

- <b>Schedule:</b>  A schema for carrying out a process or a procedure.

   - <b>None:</b> Runs immediately
   
   - <b>Repeat after completion with delay:</b> Schedule run once again with specified time delay
   
   - <b>Cron Expression:</b> It is a string consisting of 6 or 7 fields that describe individual details of the schedule. that represents a schedule. These fields, separated by white space, can contain any of the allowed values with various combinations of the allowed characters for that field.
   
><b>For instance:</b>
 ( ' 0 0 0 * * * ' ) is a daily schedule, because it matches combinations of date and time where seconds, minutes and hours are 0. If you change the hours field to 8, (' 0 0 0 8 * * * '),  your string represents every day at 8:00 AM.

| Field |Allowed Value  |Allowed Special Character|
|--|--|--|
|Seconds |  0-59|, - * /  |
|minutes|0-59|  , - * /|
|Hours|0-23|  , - * /|
|Day of month|0-31|, - * ? / L W|
|month|1-12 or JAN-DEC|  , - * /|
|Day of week|Day of week|, - * ? / L #|
|Year|1970-2099|  , - * /|

 - <b>Jobs to run after:</b> Select the job to run after your scheduled job.
 
 - <b>Tasks to run after ():</b>
 
     - <b>Sequential:</b> select sequential to run the jobs one after the other.
     
     - <b>Parallel:</b> select parallel to run the jobs parallel at the same time.
     
<b>2.</b>  Click run schedule button.

![Image 5](https://raw.githubusercontent.com/sv18042016/fp1/47f6e0897c275693ef1c3b372f71f513751c8641/images/New_version5/TD_JOBS_IMAGE5.png)
 <b><font color = "Black" >Image 5</font></b>

<b>3.</b> Click <b> Run</b> button, to run Jobs.

![Image 6](https://raw.githubusercontent.com/sv18042016/fp1/55af9eb09c6a72584a5902b13b37994e4d3dc29d/images/New_version5/TD_JOBS_IMAGE6.png)
 <b><font color = "Black" >Image 6</font></b>

<!-- ## Job Email Reports --> 

<!-- Similarly, for <b>Task Type:</b>  Email Report.

<!-- ![Image 7](https://raw.githubusercontent.com/sv18042016/fp1/30a4df6cf495b3da7f81c2ab2804d82ce4d30d49/images/New_version5/TD_JOBS_IMAGE8.png)
 <b><font color = "Black" >Image 7</font></b>

<!-- <b><i>Enter following details in Create job window;</b></i> -->

<!-- - <b>Task Type:</b> choose Email report from drop-down list. -->

<!-- - <b>Select Reports:</b> on selecting report checkbox, it will email the report result to specified email id.-->

<!-- > <b>Note</b> : you can select multiple reports at a time. -->

<!-- - <b>Select Dashboard:</b> on selecting dashboard checkbox, it will email the dashboard result to specified email id. -->

<!-- - <b>Report Layout</b>: Select the report layout using drop down list. -->

<!-- ![Image 8](https://raw.githubusercontent.com/sv18042016/fp1/59ffca65d9d61668e0299295f8bf5d33f89eafe3/images/New_version5/TD_JOBS_IMAGE9.png) -->

<!--  <b><font color = "Black" >Image 8</font></b>-->

<!-- - <b>Report Width:</b> choose report from drop down list ( large,medium and small)-->

<!-- - <b>Email Id</b> Enter email address to whom you would like to send the report.-->

<!-- - <b>Save:</b> Click on save button to save the task created.-->

<!-- <b> Note 1: </b> Navigate to <b>Gear</b> icon and click Schedule as explained above ( Refer image 5 ) and click run.-->

<!-- <b>Note 2:</b> Email recipient will receive the mail displaying the result for the report selected.-->

## Job task type ( Query Sync Full)

Under this task type data is transmitted from source to target destination, this transmitted data can be edited, updated, deleted and truncated permanently.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/79e64fae91a66f8962b7d2845e8b3c6ced52ecf0/images/New_version5/TD_JOBS_IMAGE10.png)
 <b><font color = "Black" >Image 9</font></b>

<b>Select Task Type:</b> Query sync full from drop-down list.

Enter following details in create Job window;

- <b>Source Connection:</b> Select source database connection

- <b>Query:</b> Enter the query, 

<b><i>For Instance:</i></b> in the following query summary data will be transferred to target destination
```
SELECT * FROM pragmatic.casino_summary where summary between  '${key_start}' and '${key_end}'
```
Enter following information;

<b>Block type:</b> Select <b>Date</b> from drop-down list.

- <b>Block From & To:</b>  enter start date and end date till where the data to fetched.

> <b>Block From</b> : 2019/03/01 | yyyy/MM/dd
> <b>Block To</b> : 2019/03/08 | yyyy/MM/dd

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/79e64fae91a66f8962b7d2845e8b3c6ced52ecf0/images/New_version5/TD_JOBS_IMAGE11.png)
 <b><font color = "Black" >Image10</font></b>

- <b>Block Size:</b> Enter specific run time range.

> <b>Note: Block size:</b> 3 ( on selecting 1 runs daily, 2-runs once in two days and so on)

- <b>Block Key From & To:</b> it works as reference name ( applicable in case of where conditions)

> <b>Block Key From:</b> Block Key: ${key_start}
> <b>Block Key To:</b> Block Key: ${key_end}

- <b>Target Connection:</b> Select target database connection.

- <b>Schema:</b> Select schema from drop down list.

- <b>Table:</b> Select the target table from drop down list.

  - <b>Insert/Update:</b>  Insert or update target table.
  
  - <b>Delete before insert:</b>  Delete existing data before inserting target data.
  - <b>Truncate Table before insert:</b> delete entire table before inserting target data.
  
- <b>Delete Reference Query:</b>Deletes previously existing records for blocks and reloads fresh data.

- <b>Update Reference Fields:</b>  it is a primary key based on given combination, data over writes the existing data.

- <b>Custom Field:</b>  Re-writes the give value for specified field

    - <b>Field name :</b> Enter field name for which you would like to re-write the value.
  
  -  <b>Value:</b> Enter field value to be written.
  
 
- <b>Field Mapping:</b> enable field mapping for source and target data.

> <b>Note:</b> Schedule and Run the Job

## Log

<b>4.</b> Navigate to Log window by clicking on <b>Log</b> button to view execution status.

![Im](https://raw.githubusercontent.com/sv18042016/fp1/master/images/New_version5/TD_JOBS_IMAGE7.png)
 <b><font color = "Black" >Image 11</font></b>

## Job (Query Sync Validate)
 
 Validate the data in source and target connection, choose task type <b>"Query Sync Validate."</b>

Enter below information:

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/7f80ff1486a0d724640d4bb1d1eb46f158453767/images/New_version5/TD_JOBS_IMAGE13.png)
 <b><font color = "Black" >Image 12</font></b>

- <b>Task Type:</b> Select Query Sync Validate from drop-down list.

- <b>Source Connection:</b> Select source connection.

- <b>Query:</b>  enter query to be validate in source connections.

```
SELECT * FROM pragmatic.casino_summary where summary between  '2019-03-01' and '2019-03-03'
```
- <b>Target Connection:</b> Select target connection.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/7f80ff1486a0d724640d4bb1d1eb46f158453767/images/New_version5/TD_JOBS_IMAGE14.png)
  <b><font color = "Black" >Image 13</font></b>

- <b>Target Query:</b>  enter query to be validate in target connections.
```
SELECT * FROM pragmatic.casino_summary where summary between  '2019-03-01' and '2019-03-03'
```

- <b>Field mapping:</b> Enable field mapping for source and target connection.

- Click <b>Save</b> button to save the Job. 


## Edit Job

<b>5.</b> Click <b>Edit</b> icon to edit the existing job and click on update button to save the changes.

## Delete Job

<b>6.</b> Click <b>Delete</b> icon to delete the job.

## Jobs Search option

  

Search option makes the user to work more easier as they are number of jobs in the SQL Jobs.


![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/JS1.png?raw=true)





<!--stackedit_data:
eyJoaXN0b3J5IjpbNTY4MDIwNjA5LC02NDAwNTAxMjQsLTM5Nz
MxNzQ2NSwxOTI2MzA1ODM3LC0yMTIxNTExMjE1LC0xNjQwNjc1
ODc0LDEwNDQwNDU3OSwzNzEzNDA1MzMsMTM3ODk4MjE1NywxMz
U2OTU5NjQzLC03NjM4OTc2NjAsLTE1NzgyNjE0MjAsMTQyMDcw
Nzc4MSwxNDIwNzA3NzgxLDEzMTM2MjA1NTAsLTEyNDUzOTE3MD
IsLTE5MzUzNzI4NjUsMTkyODc1MTc0MywxMTAzMDg3OTg5LDEz
Nzk3NjU5MTVdfQ==
-->