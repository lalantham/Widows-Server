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
  
  ## 03 - Install Secondary DNS Server
  	
	3.1 - Configure Static IP { It Self as a Primary DNS Server & DC Server as Secondary DNS Server }
  
 	3.2 - Change DNS Suffix to Local Domain & Tick " Use this connection DNS suffix in DNS Regstration "
  
  	3.3 - Add Secondary Server to the Domain
	  
  	3.4 - Restart Server
  
  	3.5 - In Primary DC Server -->  Add Secondary DNS Server as Newly Created DNS Server
  
  	3.6 - Add DNS Role
	
	3.7 - In Primary DC Server --> Foward Lookup Zone --> Local Domain --> Zone Transfer --> Add Secondary server 
  
 	3.8 - In Primary DC Server --> Reverse Lookup Zone --> Local Domain --> Zone Transfer --> Add Secondary server 
  
  	3.9 - Add New Foward Lookup Zone to Secondary DNS Server --> Use Secondary Server Option --> Add Local Domain Name --> Add Primary DC Server Ip
	  
  	3.10 - Add New Reverse Lookup Zone to Secondary DNS Server --> Use Secondary Server Option --> Add Primary DC Server Ip
