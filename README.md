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
After finishing the prerequisites i download the osTicket from my file folders and then exact the copy "upload" folder to c:\inetpub\wwwroot then rename upload to osTicket. After that go to IIS (internet Information Services) and restart server.
</p>
<br />

<p>
<img src="https://i.imgur.com/cXSLzxC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>	
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
