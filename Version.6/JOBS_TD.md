

<h1><center>Jobs</center></h1>

Jobs schedules a command or script on your server to run automatically at a specified time and date. Jobs are scheduled task itself, which are useful to automate repetitive tasks.

## Functionalities

- Jobs can be set to run in time interval such as by minute,hour,month,year or any of these combinations.

- You can run jobs as many times as desired.

## Getting Started

Navigate to ***SQL Runner Section***-->Jobs-->Click ***Create Job***

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/master/images/New_version5/TD_JOBS_IMAGE1.png)
 **Image**
 
 Enter the following information in Create Job Window;
 
 - **Job Name:** Name identifier for Job
 
 - **Info:** Job description
 
 - **Task Name:** Name identifier for Task
 
 - **Task Info:** Task description
 
 - **Task Type:** Select task type using drop down list

 ![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/23513febf6e72c734c80e805c286346a21504fb4/images/New_version5/TD_JOBS_IMAGE2.png)
  
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

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b679c7e6d82f09c9795d0fc4c32bbe7ef5430c8d/images/New_version5/TD_JOBS_IMAGE3.png)

## Multiple Task

Click on Task button to create multiple Task in Jobs.

## Schedule Job

**1.** Click Settings Icon available next to existing Job name and Navigate to ***Schedule.***

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/47f6e0897c275693ef1c3b372f71f513751c8641/images/New_version5/TD_JOBS_IMAGE4.png)

Under Schedule Job Window, Enter Below details;

- **Start delay:** enter time delay to run the file

- **Schedule:**

   - **None:** Runs immedietly
   - **Repeat after completion with delay:** schedule run once again with spscified time delay
   - **Cron expression:**
   
 - Jobs to run after
 - Tasks to run after
     - Sequential
     - parallel
     
**2.**  Click run schedule button.

![Image 5](https://raw.githubusercontent.com/sv18042016/fp1/47f6e0897c275693ef1c3b372f71f513751c8641/images/New_version5/TD_JOBS_IMAGE5.png)

**3.** Click Run button, to run Jobs.

![Image 6](https://raw.githubusercontent.com/sv18042016/fp1/55af9eb09c6a72584a5902b13b37994e4d3dc29d/images/New_version5/TD_JOBS_IMAGE6.png)

## Log

**4.** Navigate to Log window by clicking on **Log** button to view execution status.

![Image](https://raw.githubusercontent.com/sv18042016/fp1/master/images/New_version5/TD_JOBS_IMAGE7.png)
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5ODczMDA2NzMsLTEwNTA3NjMwNzYsLT
EwNzM4Nzk3NDVdfQ==
-->