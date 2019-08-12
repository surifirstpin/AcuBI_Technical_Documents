


<center><h2>DATABASE CONNECTION</h2></center>

 <b>Connection</b> Specifies a database connection from which a model can retrieve the data.
   
 <b>To set up database connection;</b>
    
<b>I.</b>  Get the connection details for database such as Host, Dialects, port, username, password, etc from <b>Database Administrator.</b>

<b>II.</b> Enable secure access to database, such as :
  -  Using  IP Address Whitelist, optionally adding SSL Encryption.
  - Using SSH Tunnel, which provides a secured and encrypted connection with extra authentication.
  
<b> III. </b> Set up database to work with AcuBi. Instructions may vary from dialect to dialect. Typically it includes providing approval to AcuBi to access database.

 ## Set-Up Database Connection

 Login <b>AcuBi</b> using following navigation path :

<b>Link :</b>  [http://18.196.122.102:8081/acubiLogin](http://18.196.122.102:8081/acubiLogin)

<b>Navigation: Database→ New connection</b>

 <b>1.</b> Click on <b>Database Section</b> It navigates to database connections page.

 <b>2.</b> Click on <b>New Connection</b> button  (on top right of the screen) to start setting up the connection to database. In general, specify the below mentioned fields:
  
 ![
](https://raw.githubusercontent.com/sv18042016/fp1/b9756e1483bd0d90240ab79291ca14627ae39368/images/New_version5/TD_Database_Connection_image1.png)
 <b><font color = "TEAL" >Image 1</font></b>*

***Enter the following details in New connection page ;***

-  <b>Name:</b> specify a name to define connection.
 
 - <b>Dialect:</b> choose appropriate dialect based on  connection being established. 
 
- <b>Host:</b>  Database host path.

- <b>Database:</b> Name of the database used.

- <b>Username and Password:</b> Credentials used to connect the database.

- <b>Temporary Database:</b>  To get the data path location of local files for user.

- <b>Maximum connection:</b> Concurrent connection used by  database.

- <b>Additional Parameters:</B> Additional JDBC parameter used.

## SSH 

- Enable SSH connection by select checkbox for SSH.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/ae5840d5f43f11702ee7a826f1a77aaed42ba463/images/New_version5/TD_Database_Connection_image4.png)
 <b><font color = "TEAL" >Image 2</font></b>

<b>a)</b> To connect AcuBi SSH tunnel with same database host, provide following information to AcuBi analyst :
 
  - IP address or DNS name of the database server
  - SSH port of the database server
  - Database port number
  
<b>b)</b> If connecting with separate database host, provide following information to AcuBi analyst:
  
  - IP address or DNS name of the database server as seen from the tunnel server.
  - Database port number as seen from the tunnel server.
  - IP address or DNS name of the tunnel server as seen from the public internet.
  - SSH port of the tunnel server as seen from the public internet.
  - Username and Password on the tunnel server for the SSH connection (the standard is looker).
  
  - <b>Browse Key File:</b> upload a private key for secure access.

  ![
](https://raw.githubusercontent.com/sv18042016/fp1/6098c6fb2f28bc21db1e3fe579d670fd7ff80452/images/New_version5/TD_Database_Connection_image2.png)
**Image 3**

<b>3. Dialects:</b> select the accurate dialect from the list using drop down option.

## Test and Save Connection

<b>4. Test Connection:</b> check if the entered information is running accurately.
> on hitting the test connection button, it displays a success message if all the entered information is correct, if not displays a error message. 

**5.Add Connection:** establish and save the connection.

>After establishing the connection you can see the list of connections names on left side toolbar of database section.

## Edit a connection

![
](https://raw.githubusercontent.com/sv18042016/fp1/bb8fa15c4665b7b50dbfaa9191605b04a70bfdf0/images/New_version5/TD_Database_Connection_image3.png)
**Image 4**

   **6.** Click **Edit** option to make any changes to connection established.
   
## Delete a connection

**7.** Click **Delete**  to delete the connection from database.


##  Dialects supported

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/3bbaa9982fbbf193443bb882f359d2b1cf683390/images/dialects.png)	
**Image 5**

>**Note:** Based on requirement, more dialects can be introduced in Acubi.

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE3OTIyMjI2MjMsLTE2MDQ1Nzg1ODAsLT
U3NDAxODQ3MSwtMTkyMTcxMzc5MSwtMTg3ODg2OTIyMywtMTQ0
NzU1MTU2NSwtOTQ0NTY1MDMwLDIxMTMyOTA5NTldfQ==
-->