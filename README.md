<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Install / Enable IIS in Windows WITH
CGI and Common HTTP Features
(World Wide Web Services -> Application Development Features ->
[X] CGI
[X] Common HTTP Features)

-  install/ Enable IIS Management Console
(Internet Information Services -> Web Management Tools -> IIS Management Console
	[X] IIS Management Console)

- Download and install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi) (https://drive.google.com/file/d/1RHsNd4eWIOwaNpj3JW4vzzmzNUH86wY_/view?usp=share_link)

- Download and install the Rewrite Module (rewrite_amd64_en-US.msi) (https://drive.google.com/file/d/1tIK9GZBKj1JyUP87eewxgdNqn9pZmVmY/view?usp=share_link)

- Create the directory C:\PHP
 
 -  Download PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) and unzip the contents into C:\PHP (https://drive.google.com/file/d/1snNMtLdCOpMtkCyD4mvl9yOOmvVIp9fP/view?usp=share_link)
 -  Download and install VC_redist.x86.exe. (https://drive.google.com/file/d/1s1OsGF3-ioO0_9LYizPRiVuIkb3lFJgH/view?usp=share_link)
 -  download and install MySQL 5.5.62 (mysql-5.5.62-win32.msi) (https://drive.google.com/file/d/1_OWh9p7VQLcrB0q_V7qT8yHl0xo5gv7z/view?usp=share_link)
Typical Setup ->
Launch Configuration Wizard (after install) ->
Standard Configuration ->
Password1

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/6Z3QPJM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After finishing the prerequisites download the osTicket from my file folders and then exact the copy "upload" folder to c:\inetpub\wwwroot then rename upload to osTicket. After that go to IIS (internet Information Services) and restart server.
</p>
<br />

<p>
<img src="https://i.imgur.com/cXSLzxC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
You then go to and click sites in IIS and press Default web site then press osTicket. Then on right side click Browse *80 which brings up osTicket installer on browser. Go back to IIS then in osTicket home double click PHP manager find and click on “Enable or disable an extension” enables on theses extensions php_imap.dll, php_intl.dll, php_opcache.dll Now Refresh the osTicket site in your browse, observe the changes.

</p>
<br />

<p>
<img src="https://i.imgur.com/UsSGbxw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Then rename ost-sampleconfig.php to ost-config.php go back to file explorer click open on osTicket the open include then find ost-sampleconfig.php to rename. Then right click ost-config.php the click on properties and click security then press advance at the bottom then press disable inheritance then remove all inherited premissions from this object. Then click add and click select a principal and type everyone then press check names and ok. Then press full control and ok and apply and ok again.  

<p>
 <br />
	
<img src="https://i.imgur.com/LEvbqxw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>	

Continue setting up osTicket in the browser click continue and fill out all information needed in system settings and Admin User. Now have to download and install HeidiSQL(https://docs.google.com/document/d/1WovrX2DaS9xkfaSr4LXyB4YnnWpXIgPCMMbbfgHmGVw/edit).Open HeidiSQL click new and on the right put in the passswod then press open. now need to create a database right click the blue unnamed and press create new and then database and name it osTicket after that back to the osTicket browser tpye in MySQL Database: osTicket, MySQL Username: root, and MySQL Password: Password1 then click install now and it finished installing.

</p>
<br />
<img src="https://i.imgur.com/1US9ez2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Then do a clean up by Deleting the "setup" file in C:\inetpub\wwwroot\osTicket\setup after deleteintg the "setup" file in file explorer then go to the file "include" open it and find ost-config.php go to properties and Set Permissions to “Read” only and with that the osTicket is ready to log in.


<p>
 <br />

 

