


<center><h2>DATABASE CONNECTION</h2></center>

<b>Connection</b> Specifies a database connection from which a model can retrieve the data.
   
 <b>To set up database connection, Follow the below instructions;</b>
    
<b>I.</b>  Get the connection details for database such as Host, Dialects, Port, Username, Password, etc from <b>Database Administrator.</b>

<b>II.</b> Enable secure access to database, such as :
  - Using  IP Address Whitelist, optionally adding SSL Encryption.
  - Using SSH Tunnel, which provides a secured and encrypted connection with extra authentication.
  
<b> III. </b> Set up database to work with AcuBi. Instructions may vary from dialect to dialect. Typically it includes providing approval to AcuBi to access database.

 ## Set-Up Database Connection

 Login <b>AcuBi</b> using following navigation path with your Username and Password :
 
[AcuBi Homepage Login](http://192.168.32.20:8081/acubiLogin)

<b>Navigation: Database → New connection</b>

 <b>1.</b> Click on <b>Database Section</b> It navigates to database connections page.

 <b>2.</b> Click on <b>New Connection</b> button  (on top right of the screen) to start setting up the connection to database. In general, specify the below mentioned fields:
  
 ![
](https://raw.githubusercontent.com/sv18042016/fp1/b9756e1483bd0d90240ab79291ca14627ae39368/images/New_version5/TD_Database_Connection_image1.png)
 <b><font color = "Black" >Image 1</font></b>

<b><i><u>Enter the following details in New connection page ;</u></i></b>

-  <b>Name:</b> Specify a name to define connection.
 
- <b>Dialect:</b> Choose appropriate dialect based on  connection being established. 
 
- <b>Host:</b>  Database host path.

- <b>Database:</b> Name of the database used.

- <b>Username & Password:</b> Credentials used to connect the database.

- <b>Temporary Database:</b>  To get the data path location of local files for user.

- <b>Maximum connection:</b> Concurrent connection used by  database.

Here you can set up maximum number of connections for your database


- <b>Additional Parameters:</B> Additional JDBC parameter used.

You can include here additional Java Database Connectivity (JDBC) parameters for your queries if needed.

## SSH 

Enable SSH connection by select checkbox for SSH. Select SSH encryption to protect the data as it passes between AcuBi and database. This is one way of securing your data.


![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/ae5840d5f43f11702ee7a826f1a77aaed42ba463/images/New_version5/TD_Database_Connection_image4.png)
 <b><font color = "Black" >Image 2</font></b>

<b>a)</b> To connect AcuBi SSH tunnel with same database host, provide following information to AcuBi analyst :
 
- IP address or DNS name of the database server

- SSH port of the database server
 
- Database port number
  
<b>b)</b> If connecting with separate database host, provide following information to AcuBi analyst:
  
- <b>IP address or DNS name</b> of the database server as seen from the tunnel server.
  
- <b>Database port number</b> as seen from the tunnel server.

- <b> IP address or DNS name</b> of the tunnel server as seen from the public internet.

- <b>SSH port</b> of the tunnel server as seen from the public internet.

- <b>Username and Password</b> on the tunnel server for the SSH connection (the standard is looker).
  
<b>Browse Key File:</b> upload a private key for secure access.

  ![
](https://raw.githubusercontent.com/sv18042016/fp1/6098c6fb2f28bc21db1e3fe579d670fd7ff80452/images/New_version5/TD_Database_Connection_image2.png)
<b><font color = "Black" >Image 3</font></b>

<b>3. Dialects:</b> select the accurate dialect from the list using drop down option.

AcuBi allows wide range of SQL database dialects and will continue to improve the feature implementation for existing dialects used as well as for newly added dialects.


## Test and Save Connection

<b>4. Test Connection:</b> To check wearher the entered information is running accurately and weather the database is able to connect.

> On hitting test connection button, it displays a success message if entered information is correct, if not displays a error message. 

<b>5. Add Connection:</b> Establish and save the connection.

>After establishing the connection you can see the list of connections names on left side toolbar of database section.

## Edit Connection

![
](https://raw.githubusercontent.com/sv18042016/fp1/bb8fa15c4665b7b50dbfaa9191605b04a70bfdf0/images/New_version5/TD_Database_Connection_image3.png)
<b><font color = "Black" >Image 4</font></b>

   <b>6.</b> Click <b>Edit</b> option to make any changes to connection established.
   
## Delete a connection

<b>7.</b>Click <b> Delete</b>  to delete the connection from database.

##  Dialects supported

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/3bbaa9982fbbf193443bb882f359d2b1cf683390/images/dialects.png)	
  <b><font color = "Black" >Image 5</font></b>

><b> Note:</b> Based on requirement, more dialects can be introduced in Acubi.

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTY5MDczNDY2NiwxMDM5MzI1NTAwLDM1Mz
k3NTc5NCwtMTIxMjQ5NzMxMiwxOTgwMTg1ODE4LC0xNDA5MjM5
NDQzLDE4NzU0OTA3MzEsLTE2Nzk4ODYzNTYsMjEzODQ1ODU0Ni
wtMTM2MjQxMTU5LDY0ODAwMjQ1NCw3MDUwNDQ5NjEsMzk1NTk3
MTIzLDE2Mjk3Nzc5NTQsMTIwOTIyOTkyMl19
-->