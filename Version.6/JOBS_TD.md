

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

- **Query:** write a query for update,insert,delete or truncate records.

- **Global Block:** it is enabled, to repeat same job for all the task.

- **Block Type:** Choose block type Number,Hour and Date.

- **Block From & To:**  Enter the start and the ending point of the data to be fetched.

- **Block Size:** Enter specific run time range.

- **Block Key From & To:** it works as reference name ( applicable in case of where conditions)

Click Save, to save the Job created.

All the saved jobs are visible under SQL Jobs list.

![Image 3](https://raw.githubusercontent.com/sv18042016/fp1/b679c7e6d82f09c9795d0fc4c32bbe7ef5430c8d/images/New_version5/TD_JOBS_IMAGE3.png)
**Image 3**

## Multiple Task

Click on Task button to create multiple Task in Jobs.

## Schedule Job

**1.** Click Settings Icon available next to existing Job name and Navigate to ***Schedule.***

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/47f6e0897c275693ef1c3b372f71f513751c8641/images/New_version5/TD_JOBS_IMAGE4.png)

Under Schedule Job Window, Enter Below details;

- **Start delay:** enter time delay to run the file

- **Schedule:**

   - **None:** Runs immediately
   
   - **Repeat after completion with delay:** schedule run once again with spscified time delay
   
   - **Cron expression:** it is a string consisting of 6 or 7 fields that describe individual details of the schedule. that represents a schedule. These fields, separated by white space, can contain any of the allowed values with various combinations of the allowed characters for that field.
   
>**For instance:**
The string represents a set of times, which are the times that match the CRON expression. For example, ( ' 0 0 0 * * * ' ) is a daily schedule, because it matches combinations of date and time where seconds, minutes and hours are 0. If you change the hours field to 8, (' 0 0 0 8 * * * '),  your string represents every day at 8:00 AM.

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

**3.** Click Run button, to run Jobs.

![Image 6](https://raw.githubusercontent.com/sv18042016/fp1/55af9eb09c6a72584a5902b13b37994e4d3dc29d/images/New_version5/TD_JOBS_IMAGE6.png)

## Job Email Reports

Similarly

## Log

**4.** Navigate to Log window by clicking on **Log** button to view execution status.

![Image](https://raw.githubusercontent.com/sv18042016/fp1/master/images/New_version5/TD_JOBS_IMAGE7.png)

## Edit Job
**5.** Click Edit icon to edit the existing job and click on update button to save the changes.

## Delete Job

**6.** Click Delete icon to delete the job.


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTMwNDc5MDQwOCw1MjI0MTY1OTgsOTY4Nz
Q4OTY0LC0xMDUwNzYzMDc2LC0xMDczODc5NzQ1XX0=
-->