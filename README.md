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
<img src="https://imgur.com/MAhXK2e.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://imgur.com/Zf2jw07.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Now that your in the VM you'll want to open control panel, go to programs, turn Windows features on or off, and then enable Internet Information Services, Web Management Tools, World Wide Web Services.
- Next up open World Wide Web Services and enable Application Development Features, Common HTTP Features (Make sure everything within this is checked), Health and Diagnostics, Performance Features, and Security.
- And finally open up Application Development Features and check off CGI. Now hit okay and wait for the changes to happen, if everything is installed and enabled correctly then if you go to your browser of choice and search for 127.0.0.1 it should open up to this page.

<p></p>

- Now that we have the files downloaded and installed we will want to search for IIS in the windows search bar and then open it AS AN ADMINISTRATOR.
- 
