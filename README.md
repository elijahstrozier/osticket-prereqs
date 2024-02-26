<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket with CourseCareers.<br />






<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Install / Enable IIS in Windows WITH CGI and Common HTTP Features AND IIS Management Console

- Installing MySQL 5.5.62

- Creating a directory for PHP

- Registering PHP from within IIS



<h2>Installation Steps</h2>
Install / Enable IIS in Windows WITH CGI and Common HTTP Features World Wide Web Services -> Application Development Features ->
[X] CGI [X] Common HTTP Features AND IIS Management Console Internet Information Services -> Web Management Tools -> IIS Management Console
[X] IIS Management Console


![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/39d375cf-543c-493f-a651-c55891459713)


![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/c448ed00-ccb9-4e00-82c3-1a3108b224cf)


![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/556d561a-f78f-4cf4-a429-8106c0b9ef01)

From the Installation Files, download and install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)
From the Installation Files, download and install the Rewrite Module (rewrite_amd64_en-US.msi)
Create the directory C:\PHP
From the Installation Files, download PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) and unzip the contents into C:\PHP
Register PHP from within IIS
Install osTicket v1.15.8. Download osTicket from the Installation Files Folder. Extract and copy “upload” folder to c:\inetpub\wwwroot
Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”
Reload IIS (Open IIS, Stop and Start the server)
Go to sites -> Default -> osTicket
On the right, click “Browse *:80”

Note that some extensions are not enabled
Go back to IIS, sites -> Default -> osTicket
Double-click PHP Manager
Click “Enable or disable an extension”
Enable: php_imap.dll
Enable: php_intl.dll
Enable: php_opcache.dll
Refresh the osTicket site in your browse, observe the changes


![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/e260c1a9-c4c0-4834-829a-f3400091cbd5)


![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/4a67ff5d-19fd-4a9e-b868-2dcdcb2d06ae)


![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/ec4ad05b-dbef-4755-a79c-8da4a794d1b4)


![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/26180948-fe9d-482b-b429-4af69f003de1)

