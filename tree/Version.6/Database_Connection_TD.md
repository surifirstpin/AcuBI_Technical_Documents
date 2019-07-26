


<center><h2>DATABASE CONNECTION</h2></center>

 **Connection** Specifies a database connection from which a model can retrieve the data.
   
 **To set up database connection;**
    
**I.**  Get the connection details for database such as Host, Dialects, port, username, password, etc from **Database Administrator.**

**II.** Enable secure access to database, such as :
  -  Using  IP Address Whitelist, optionally adding SSL Encryption.
  - Using SSH Tunnel, which provides a secured and encrypted connection with extra authentication.
  
**III.** Set up database to work with AcuBi. Instructions may vary from dialect to dialect. Typically it includes providing approval to AcuBi to access database.

 ## Set-Up Database Connection

 Login **AcuBi** using following navigation path :

**Link :**  [http://18.196.122.102:8081/acubiLogin](http://18.196.122.102:8081/acubiLogin)

>**Navigation: Database→ New connection**

 **1.** Click on **Database Section.** It navigates to database connections page.

 **2.** Click on **New Connection** button  (on top right of the screen) to start setting up the connection to database. In general, specify the below mentioned fields:
  
 ![
](https://raw.githubusercontent.com/sv18042016/fp1/b9756e1483bd0d90240ab79291ca14627ae39368/images/New_version5/TD_Database_Connection_image1.png)
**Image 1**

***Enter the following details in New connection page ;***

-  **Name** specify a name to define connection.
 
 - **Dialect** choose appropriate dialect based on  connection being established. 
 
>**Note:** Depending on priority, more number of dialects can be introduced in Acubi.

- **Host**  Database host path.

- **Database** Name of the database used.

- **Username and Password** Credentials used to connect the database.

- **Temporary Database**  To get the data path location of local files for user.

- **Maximum connection** Concurrent connection used by  database.

- **Additional Parameters** Additional JDBC parameter used.

## SSH 
- Enable SSH connection by select checkbox for SSH.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/ae5840d5f43f11702ee7a826f1a77aaed42ba463/images/New_version5/TD_Database_Connection_image4.png)

**a)**  To connect AcuBi SSH tunnel with same database host, provide following information to AcuBi analyst :
 
  - IP address or DNS name of the database server
  - SSH port of the database server
  - Database port number
  
**b)** If connecting with separate database host, provide following information to AcuBi analyst:
  
  - IP address or DNS name of the database server as seen from the tunnel server.
  - Database port number as seen from the tunnel server.
  - IP address or DNS name of the tunnel server as seen from the public internet.
  - SSH port of the tunnel server as seen from the public internet.
  - Username and Password on the tunnel server for the SSH connection (the standard is looker).
  - **Browse Key File** upload a private key for secure access.

  ![
](https://raw.githubusercontent.com/sv18042016/fp1/6098c6fb2f28bc21db1e3fe579d670fd7ff80452/images/New_version5/TD_Database_Connection_image2.png)
**Image 2**

**3.** **Dialects** select the accurate dialect from the list using drop down option.

## Test and Save Connection

**4.** **Test Connection** check if the entered information is running accurately.
> on hitting the test connection button, it displays a success message if all the entered information is correct, if not displays a error message. 

**5.** **Add Connection** establish and save the connection.

>After establishing the connection you can see the list of connections names on left side toolbar of database section.

## Edit a connection

![
](https://raw.githubusercontent.com/sv18042016/fp1/bb8fa15c4665b7b50dbfaa9191605b04a70bfdf0/images/New_version5/TD_Database_Connection_image3.png)
**Image 3**

   **6.** Click **Edit** option to make any changes to connection established.
   
## Delete a connection

**7.** Click **Delete**  to delete the connection from database.


##  Dialects supported

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/3bbaa9982fbbf193443bb882f359d2b1cf683390/images/dialects.png)	

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTY0Mzk1Mjg2NCwtOTQ0NTY1MDMwLDIxMT
MyOTA5NTksLTExOTAyNTExMTNdfQ==
-->