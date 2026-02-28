# osticket-prereqs

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine
- Internet Information Services (IIS)
- PHP Manager
- Rewrite Module
- VC Redist
- MySQL
- Heidi SQL
- osTicket v1.15.8
- Link to downloads: https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6

<h2>Installation Steps</h2>

- First off you'll need to set up an Azure Resource Group and a Virtual Machine (VM). For this I'll be using Windows 10 Enterprise version 22H2 x64 Gen2. Once you have created your resource group and your virtual machine you'll have to turn on the VM if it's turned off then log into it.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

- Now that your in the VM you'll want to open control panel, go to programs, turn Windows features on or off, and then enable Internet Information Services, Web Management Tools, World Wide Web Services.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

- Next up open World Wide Web Services and enable Application Development Features, Common HTTP Features (Make sure everything within this is checked), Health and Diagnostics, Performance Features, and Security.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

- And finally open up Application Development Features and check off CGI. Now hit okay and wait for the changes to happen, if everything is installed and enabled correctly then if you go to your browser of choice and search for 127.0.0.1 it should open up to this page.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

<p></p>

- Now that Internet Information Services, or IIS for short, is enabled we'll be downloading and installing everything we need from within the Google Drive.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

- First off you'll download and install PHP Manager for IIS, next we'll go through the install wizard and complete the install.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

- Now that we're done with that, next up we'll be installing the Rewrite Module and go through it's installation.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

- Now create a folder in the C drive called PHP and from the installation files download PHP 7.3.8 and unzip it's contents into C:\PHP

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

- Once you have downloaded and extracted the zip file into the PHP folder on the C drive, download and install the VC_redist.x86.exe and go through the setup wizard for it.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

- And finally download and install MySQL 5.5.62 and run the setup wizard, this one I'll have to guide you through for this. Select Typical Setup, Launch Configuartion Wizard (after it installs), then Standard Configuration.
As for the root password, just type in root. And finally click execute on it's all done.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

- Now that we have the files downloaded and installed we will want to search for IIS in the windows search bar and then open it AS AN ADMINISTRATOR.
- Next click on PHP Manager and register new PHP version. We'll want to provide a path to the php executable file to we'll be going to C drive, Php, and click on the php-cgi file.
Once that's done we'll restart the IIS server.
- We'll now want to install osTicket v1.15.8, download osTicket from the installation files folder, extract and copy the "upload' folder to C:\inetpub\wwwroot then from within this folder rename "upload" into "osTicket" and have it spelled that exact way.
Then we'll reload IIS again.
