<h1><center>Two Factor Authentication</center> </h1>

  

<b> Functionality :  </b> Two factor authentication shortly known as 2FA is a authorization mechanism where 6 didgit OTP (One Time Password) is generated using Google Authenticator mobile app.This google authenticator generates code for every 30 seconds.

  

<b> Interpretation :  </b> Now a days cracking a password is happening in many applications and much fraud can be done. To overcome this issue we are providing Two factor authentication through Google Authenticator app which creates/ refresh a new code for every 30 seconds, Even after login through given credentials one more security check in the form of 6 didgit code is insisted to access ACUBI . As the code refereshes for every 30 seconds so the maximum length of the session at 2FA is limited to 30 seconds.Once logout and login again system prompts for new password.This is where two-factor authentication comes in handy and make attacker’s life harder and reduce fraud risks.

  

<b> Process :  </b>

  

-   For setting up two-factor authentication to an ACUBI account the user name should be a valid email address.
    

-   Once 2FA is enabled for an account sysytem generates a email as shown in below figure
    

and then Click on <b> Display now </b> 

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/2FA%201.png?raw=true)<b><font color = "Black" >Image </font></b>

-   It generates a bar code as shown below .

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/2FA%202.png?raw=true)<b><font color = "Black" >Image </font></b>

-   Through Google authenticator app we need register the account by scanning the bar code .



![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/2FA%203.png?raw=true)<b><font color = "Black" >Image </font></b>
  

-   This 6 digit code is applied in 2FA as shown below.

![enter image description here](https://github.com/surifirstpin/AcuBI_Technical_Documents/blob/master/images/2FA%204.png?raw=true)
<b><font color = "Black" >Image </font></b>


-   Once the code is applied can access ACUBI site.
<!--stackedit_data:
eyJoaXN0b3J5IjpbOTA2Mjc4NjEyLDE4NDQ3MzYzNDAsLTEyMT
MxNzM2MzAsMTYwODMyMTk3NiwtNTYyNDU1MjkwXX0=
-->