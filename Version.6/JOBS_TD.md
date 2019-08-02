

<h1><center>Jobs</center></h1>

Jobs schedules a command or script on your server to run automatically at a specified time and date. Jobs are scheduled task itself, which are useful to automate repetitive tasks.

## Functionalities

- Jobs can be set to run in time interval such as by minute,hour,month,year or any of these combinations.

- You can run jobs as many times as desired.

## Getting Started with Job for 

Navigate to ***SQL Runner Section***-->Jobs-->Click ***Create Job***

![Image 1](https://raw.githubusercontent.com/sv18042016/fp1/master/images/New_version5/TD_JOBS_IMAGE1.png)

 **Image 1**
 
 Enter the following information in Create Job Window;
 
 - **Job Name:** Name identifier for Job
 
 - **Info:** Job description
 
 - **Task Name:** Name identifier for Task
 
 - **Task Info:** Task description
 
 - **Task Type:** Select task type using drop down list

 ![Image 2](https://raw.githubusercontent.com/sv18042016/fp1/23513febf6e72c734c80e805c286346a21504fb4/images/New_version5/TD_JOBS_IMAGE2.png)

 **Image 2**
  
***For Instance:*** in this document, i am creating a Job for task type-Query Execute.

On selecting Query Execute, it display following functionalities;

- **Source Connection:** Select database connection used.

- **Query:** Enter your query.

- **Global Block:** it is enabled, to repeat same job for all the task.

- **Block Type:** Choose block type Number,Hour and Date.

- **Block From & To:**  Enter the start and the ending point of the data to be fetched.

- **Block Size:** Enter specific run time range.

- **Block Key From & To:** it works as reference name ( applicable in case of where conditions)

Click **Save**, to save the Job created.

All the saved jobs are visible under SQL Jobs list.

![Image 3](https://raw.githubusercontent.com/sv18042016/fp1/b679c7e6d82f09c9795d0fc4c32bbe7ef5430c8d/images/New_version5/TD_JOBS_IMAGE3.png)

**Image 3**

## Multiple Task

Click on Task button to create multiple Task in Jobs.

## Schedule Job

**1.** Click Settings Icon available next to existing Job name and Navigate to ***Schedule.***

![Image 4](https://raw.githubusercontent.com/sv18042016/fp1/47f6e0897c275693ef1c3b372f71f513751c8641/images/New_version5/TD_JOBS_IMAGE4.png)

**Image 4**

Under Schedule Job Window, Enter Below details;

- **Start delay:** enter time delay to run the file

- **Schedule:**

   - **None:** Runs immediately
   
   - **Repeat after completion with delay:** schedule run once again with specified time delay
   
   - **Cron expression:** it is a string consisting of 6 or 7 fields that describe individual details of the schedule. that represents a schedule. These fields, separated by white space, can contain any of the allowed values with various combinations of the allowed characters for that field.
   
>**For instance:**
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

 - **Jobs to run after:** Select the job to run after your scheduled job.
 
 - **Tasks to run after():**
 
     - **Sequential:** select sequential to run the jobs one after the other.
     
     - **Parallel:** select parallel to run the jobs parallel at the same time.
     
**2.**  Click run schedule button.

![Image 5](https://raw.githubusercontent.com/sv18042016/fp1/47f6e0897c275693ef1c3b372f71f513751c8641/images/New_version5/TD_JOBS_IMAGE5.png)

**Image 5**

**3.** Click Run button, to run Jobs.

![Image 6](https://raw.githubusercontent.com/sv18042016/fp1/55af9eb09c6a72584a5902b13b37994e4d3dc29d/images/New_version5/TD_JOBS_IMAGE6.png)

**Image 6**

## Job Email Reports

Similarly for task type **Email Reports**

![Image 7](https://raw.githubusercontent.com/sv18042016/fp1/30a4df6cf495b3da7f81c2ab2804d82ce4d30d49/images/New_version5/TD_JOBS_IMAGE8.png)

**Image 7**

***Enter following details in Create job window;***

- **Task Type:** choose Email report from drop-down list.

- **Select Reports:** on selecting report checkbox, it will email the report result to specified email id.

> **Note** : you can select multiple reports at a time.

- **Select Dashboard:** on selecting dashboard checkbox, it will email the dashboard result to specified email id.

- **Report Layout**: Select the report layout using drop down list.

![Image 8](https://raw.githubusercontent.com/sv18042016/fp1/59ffca65d9d61668e0299295f8bf5d33f89eafe3/images/New_version5/TD_JOBS_IMAGE9.png)

**Image 8**

- **Report Width:** choose report from drop down list ( large,medium and small)

<font color = orange> **Filter Json:**  ?????


- **Email Id** Enter email address to whom you would like to send the report.

- **Save:** Click on save button to save the task created.

Navigate to settings icon and click Schedule as explained above ( Refer image 5 ) and click run.

**Note:** Email recipient will receive the mail displaying the result for the report selected.

## Job task type ( Query Sync Full)

under this task type data is transmitted from source to target destination, this transmitted data can be edited, updated, deleted and truncated permanently.

**Select task type** : Query sync full from drop-down list.

Enter following details in create Job window;

- **Source Connection:** select source database connection

- **Query:** Enter the query, 

**For Instance:** in the following query summary data will be transferred to target destination
```
SELECT * FROM pragmatic.casino_summary where summary between  '${key_start}' and '${key_end}'
```



## Log

**4.** Navigate to Log window by clicking on **Log** button to view execution status.

![Image](https://raw.githubusercontent.com/sv18042016/fp1/master/images/New_version5/TD_JOBS_IMAGE7.png)


## Edit Job

**5.** Click Edit icon to edit the existing job and click on update button to save the changes.

## Delete Job

**6.** Click Delete icon to delete the job.


<!--stackedit_data:
eyJoaXN0b3J5IjpbNTI2MDk1Nzg3LDExNDgzODYwNTUsLTE5Nz
EzMTQxNTgsMTU1ODk2NzMxNSwtNDAyMjYyNzkxLC0yMDc4MTE1
MDA5LDE0MDYzNDM4ODksMTQ1ODE1MTEyOSwxMjk4NDYxODk1LD
MyNjAwNTQ2Nyw4OTM1MzQ0MTksMTMwNDc5MDQwOCw1MjI0MTY1
OTgsOTY4NzQ4OTY0LC0xMDUwNzYzMDc2LC0xMDczODc5NzQ1XX
0=
-->