

<h1><center>Jobs</center></h1>

Jobs are used for scheduling tasks to run on the server. They are most commonly used for automating system maintenance or administration at a specified time and date. Jobs are scheduled task itself, which are useful to automate repetitive tasks.

## Functionalities

- Jobs can be set to run in time interval such as by minute,hour,month,year or any of these combinations.

- You can run jobs as many times as desired.

## Getting Started 

Navigate to ***SQL Runner Section***-->Jobs-->Click ***Create Job***

![Image 1](https://raw.githubusercontent.com/sv18042016/fp1/master/images/New_version5/TD_JOBS_IMAGE1.png)

<b><font color = "TEAL" >Image 1</font></b>
 
 Enter the following information in Create Job Window;
 
 - <b>Job Name:</b> Name identifier for Job
 
 - <b>Info:</b> Job description
 
 - <b>Task Name:</b> Name identifier for Task
 
 - <b>Task Info:</b> Task description
 
 - <b>Task Type:</b> Select task type using drop down list.

 ![Image 2](https://raw.githubusercontent.com/sv18042016/fp1/23513febf6e72c734c80e805c286346a21504fb4/images/New_version5/TD_JOBS_IMAGE2.png)

 <b><font color = "TEAL" >Image 2</font></b>
  
<b>For Instance:</b> in this document, i am creating a Job for task type-->Query Execute.

On selecting Query Execute, it display following functionalities;

- <b>Source Connection:</b> Select database source connection.

- <b>Query:</b> Enter your query.

- **Global Block:** on selecting the checkbox for global block, the global type condition is applied for multiple tasks available under existing Job.

- <b>Block Type:</b> Choose block type Number, Hour and Date.

- <b>Block From & To:</b>  Enter the start and the ending point of the data to be fetched.

- <b>Block Size:</b> Enter specific run time range.

- <b>Block Key From & To:</b> it works as reference name ( applicable in case of where conditions)

Click <b>Save,</b> to save the Job created.

All the saved jobs are visible under SQL Jobs list.

![Image 3](https://raw.githubusercontent.com/sv18042016/fp1/b679c7e6d82f09c9795d0fc4c32bbe7ef5430c8d/images/New_version5/TD_JOBS_IMAGE3.png)

**Image 3**

## Multiple Task

Click on Task button to create multiple Task in Jobs.

## Schedule Job

**1.** Click Settings Icon available next to existing Job name and Navigate to <b><i>Schedule.</i></b>

![Image 4](https://raw.githubusercontent.com/sv18042016/fp1/47f6e0897c275693ef1c3b372f71f513751c8641/images/New_version5/TD_JOBS_IMAGE4.png)

**Image 4**

Under Schedule Job Window, Enter Below details;

- <b>Start delay:</b> enter time delay to run the file

- <b>Schedule:</b>

   - <b>None:</b> Runs immediately
   
   - <b>Repeat after completion with delay:</b> schedule run once again with specified time delay
   
   - <b>Cron expression:</b> it is a string consisting of 6 or 7 fields that describe individual details of the schedule. that represents a schedule. These fields, separated by white space, can contain any of the allowed values with various combinations of the allowed characters for that field.
   
><b>For instance:</b>
 ( ' 0 0 0 * * * ' ) is a daily schedule, because it matches combinations of date and time where seconds, minutes and hours are 0. If you change the hours field to 8, (' 0 0 0 8 * * * '),  your string represents every day at 8:00 AM.

| Field |Allowed Value  |Allowed Special Character|
|--|--|--|
| Seconds |  0-59|, - * /  |
|minutes|0-59|  , - * /|
|Hours|0-23|  , - * /|
|Day of month|0-31|, - * ? / L W|
|month|1-12 or JAN-DEC|  , - * /|
|Day of week|Day of week|, - * ? / L #|
|Year|1970-2099|  , - * /|

 - <b>Jobs to run after:</b> Select the job to run after your scheduled job.
 
 - <b>Tasks to run after():</b>
 
     - <b>Sequential:</b> select sequential to run the jobs one after the other.
     
     - <b>Parallel:</b> select parallel to run the jobs parallel at the same time.
     
**2.**  Click run schedule button.

![Image 5](https://raw.githubusercontent.com/sv18042016/fp1/47f6e0897c275693ef1c3b372f71f513751c8641/images/New_version5/TD_JOBS_IMAGE5.png)

**Image 5**

**3.** Click <b> Run</b> button, to run Jobs.

![Image 6](https://raw.githubusercontent.com/sv18042016/fp1/55af9eb09c6a72584a5902b13b37994e4d3dc29d/images/New_version5/TD_JOBS_IMAGE6.png)

**Image 6**

## Job Email Reports

Similarly for task type <b>Email Report.</b>

![Image 7](https://raw.githubusercontent.com/sv18042016/fp1/30a4df6cf495b3da7f81c2ab2804d82ce4d30d49/images/New_version5/TD_JOBS_IMAGE8.png)

**Image 7**

<b><i>Enter following details in Create job window;</b></i>

- <b>Task Type:</b> choose Email report from drop-down list.

- <b>Select Reports:</b> on selecting report checkbox, it will email the report result to specified email id.

> <b>Note</b> : you can select multiple reports at a time.

- <b>Select Dashboard:</b> on selecting dashboard checkbox, it will email the dashboard result to specified email id.

- <b>Report Layout</b>: Select the report layout using drop down list.

![Image 8](https://raw.githubusercontent.com/sv18042016/fp1/59ffca65d9d61668e0299295f8bf5d33f89eafe3/images/New_version5/TD_JOBS_IMAGE9.png)

**Image 8**

- <b>Report Width:</b> choose report from drop down list ( large,medium and small)

- <b>Email Id</b> Enter email address to whom you would like to send the report.

- <b>Save:</b> Click on save button to save the task created.

<b> Note 1: </b> Navigate to settings icon and click Schedule as explained above ( Refer image 5 ) and click run.

<b>Note 2:</b> Email recipient will receive the mail displaying the result for the report selected.

## Job task type ( Query Sync Full)

under this task type data is transmitted from source to target destination, this transmitted data can be edited, updated, deleted and truncated permanently.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/79e64fae91a66f8962b7d2845e8b3c6ced52ecf0/images/New_version5/TD_JOBS_IMAGE10.png)
**Image 9**

**Select task type** : Query sync full from drop-down list.

Enter following details in create Job window;

- **Source Connection:** select source database connection

- **Query:** Enter the query, 

**For Instance:** in the following query summary data will be transferred to target destination
```
SELECT * FROM pragmatic.casino_summary where summary between  '${key_start}' and '${key_end}'
```
Enter following information;

**Block type:** Select ***Date*** from drop-down list.

- **Block From & To:**  enter start date and end date till where the data to fetched.

> **Block from** : 2019/03/01 | yyyy/MM/dd
> **Block To** : 2019/03/08 | yyyy/MM/dd

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/79e64fae91a66f8962b7d2845e8b3c6ced52ecf0/images/New_version5/TD_JOBS_IMAGE11.png)

**Image 10**


- **Block Size:** Enter specific run time range.

> Block size : 3 ( on selecting 1 runs daily, 2-runs once in two days and so on)

- **Block Key From & To:** it works as reference name ( applicable in case of where conditions)

> **Block Key From:** Block Key: ${key_start}
> **Block Key To:** Block Key: ${key_end}

- **Target Connection:** select target database connection.

- **Schema:** select schema from drop down list.

- **Table:** select the target table from drop down list.

  - **Insert/Update:**  insert or update target table.
  
  - **Delete before insert:**  delete existing data before inserting target data.

  - **Truncate Table before insert:** delete entire table before inserting target data.
  
- **Delete Reference Query:** deletes previously existing records for blocks and reloads fresh data.

- **Update Reference Fields:**  it is a primary key based on given combination, data over writes the existing data.

- **Custom Field:**  re-writes the give value for specified field

    - **Field name :** enter field name for which you would like to re-write the value.
  
  *   **Value:** enter field value to be written.
  
 
- **Field Mapping:** enable field mapping for source and target data.

> **Note:** Schedule and Run the Job

## Log

**4.** Navigate to Log window by clicking on **Log** button to view execution status.

![Im](https://raw.githubusercontent.com/sv18042016/fp1/master/images/New_version5/TD_JOBS_IMAGE7.png)

**Image 11**

## Job (Query Sync Validate)
 
 Validate the data in source and target connection, choose task type ***"Query Sync Validate."***

Enter below information:

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/7f80ff1486a0d724640d4bb1d1eb46f158453767/images/New_version5/TD_JOBS_IMAGE13.png)

**Image 12**

- **Task Type:** Select Query Sync Validate from drop-down list.

- **Source Connection:** Select source connection.

- **Query:**  enter query to be validate in source connections.

```
SELECT * FROM pragmatic.casino_summary where summary between  '2019-03-01' and '2019-03-03'
```
- **Target Connection:** Select target connection.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/7f80ff1486a0d724640d4bb1d1eb46f158453767/images/New_version5/TD_JOBS_IMAGE14.png)

**Image 13**

- **Target Query:**  enter query to be validate in target connections.
```
SELECT * FROM pragmatic.casino_summary where summary between  '2019-03-01' and '2019-03-03'
```

- **Field mapping:** Enable field mapping for source and target connection.

- Click **Save** button to save the Job. 


## Edit Job

**5.** Click Edit icon to edit the existing job and click on update button to save the changes.

## Delete Job

**6.** Click Delete icon to delete the job.


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIxMDQ5OTk0NTEsLTE1ODIwNzkzNjksMT
g5ODg4NDUxMCwxNzY1OTExMDgxLDE4OTA0Mjg2MzMsLTI5MTc1
MTI1NCwxNDI3NTEwMDU4LDk2Mzg0NDE5OCw0MzMwMTA1MTQsNT
U0MTQwOTc0LC0xMTYxMTM2ODQ4LDEzODk1NjE4NDksNDQ5NzY0
MzU5LC0xMjkyMjgwNDc3LDM4MzMyMTI2MiwyMTAyNTYxNDA5LD
E4MzkwNDc5NCwyMTE2MTczMjE3LC0xMzkyMDAzODk3LC0xOTA5
OTU3NzIyXX0=
-->