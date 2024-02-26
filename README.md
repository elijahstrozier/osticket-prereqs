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

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/5e8fb00b-e8ba-4109-bb9f-c2587d6df5b8)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/93a6c1bb-97ec-41dd-b4d8-ef039b53cdd8)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/173532e2-5cd0-4e40-8dc8-8024188090c9)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/66757b24-cc3d-478f-84fc-3b39382f0b55)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/3704f43d-fe3b-4034-9454-b164da8a6764)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/e584c0e6-7450-4df5-a325-0dcb80bec47b)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/f153a86e-d663-48b6-97fe-c33d570bb663)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/ffd5d546-177b-48c0-8e33-9d298d637b65)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/d2ad3227-a971-489c-9101-ef9231809a2b)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/f9240d6b-76bc-45a2-8547-0b0dd941f585)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/de321fde-1f01-4a08-8600-5b89032fdfac)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/3f499e37-6024-4543-86f7-31dbaa8d550f)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/b372479c-6d07-440d-9fca-545c8765bbf3)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/3a11549d-da4d-4ab8-bdee-b0aeb21a4dd2)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/e6247ca8-8a5c-464b-8e3e-88def68864a7)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/d90be410-1fad-4e53-812a-0e32eb142407)



![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/646b0174-3557-4b32-9a48-4b1b5ce5ee6a)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/f076d86b-806f-409f-9e3c-a9de604cc479)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/26180948-fe9d-482b-b429-4af69f003de1)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/f31d4e17-aee7-4acc-8444-592d85eae25c)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/bb8668ef-db3d-40ce-be47-4b254e980a46)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/b059a6bb-dfcb-49f1-ad4e-5dc90f4cd2e8)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/67ae6d9c-397f-430f-afb5-145455e4e163)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/2eb82d6f-fe29-49b7-98b1-f05c2227a208)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/2da5337e-4f7b-4ad2-bd4f-2c3dfe0ab699)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/b944db56-9f41-4275-8aa8-e9e6925084c7)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/078ae247-c9f5-4594-a69b-9e91c9f52a12)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/a94f3b04-5e59-4556-80fe-7a421488dd0e)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/0175ad9a-5ff2-46f3-a984-9cf4d9f0a3b3)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/c467ae3b-4ad7-417a-8a40-43bbe3a7d07c)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/a97af9b8-3b76-44b0-88b5-642c3fd47e14)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/dcae5546-9ead-4265-a6f2-92f610d6a683)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/2edc904d-b245-492b-a248-81746a2e287b)

![image](https://github.com/elijahstrozier/osticket-prereqs/assets/161254320/7daa9ab7-509c-4f0a-86ef-ce612970879d)







