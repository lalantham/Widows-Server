![Repo Image](https://github.com/lalantham/Widows-Server/blob/master/winserver.jpg)
# Instal and Configure Windows Server

>Complete Guild for Instal and Configure Windows Server

## 01 - Install Instal Windows Server Os

	1.1 - Put Strong Admin Password

	1.2 - Rename Server to Proper Name	  

	1.3 - Assign Static Ip { with DNS Serer - same ip in DC Controler }

## 02 - Install Active Directory

	2.1 - Install Active Directory Domain Services { Add Role and Feature }
  
 	2.2 - Check restart if needed { optional }
  
  	2.3 - Promote the Server as Domain Contoler
          - Add New Forest --> Put Root Domain Name
          - Set Proper Domain and Forest Functional Levels
          - Set DSRM Password { Directory Service Restore Mode }
          - Proceed Installation Process
	  
  	2.4 - Restart Server
  
  	2.5 - Create Reverse Lookup Zone --> With Defaults
  
  	2.6 - Foward Lookup Zone --> Server Name --> Properties --> Update Associated Pointer
  
  
