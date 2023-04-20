<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine
- osTicket Installation files
- Heidi SQL

<h2>Installation Steps</h2>

Welcome to my first tutorial!

First we will have to create a Virtual machine using the Microsoft Azure portal. We will be using a VM which is a remote computer. We are using a VM in order to protect our physical machine just in case something breaks. We will create a resource group and title it "osTicket". Afterwards creating a VM with 2-4 CPUs. In this example we will be using 4 CPUs.

<p>
<img src="https://i.imgur.com/DZyFdnX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 

 
<p>
<img src="https://imgur.com/6iwd13Q" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 

  <p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

<h2>Installation Steps</h2>

Enable IIS (Internet Information Services)

Install  Web Platform Installer

Install MySQL

Set up User Name and Password

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>


Next simply connect to your newly created VM (Virtual Machine) using RDC (Remote DesktopConnection) using the public IPv4 address. If you are a Mac user you will have to download Microsoft RDC.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Now that you are connected to your VM you will have to enable IIS. Simply access the control panel then select uninstall a program. Off to the left select "Turn windows features on/off". A list will appear then you will enable Internet Information Services.
<p>
<p>
<img src="https://i.imgur.com/OPaIGoN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Excellent. Now that you have enabled IIS we need to install Web Platform Installer. I have provided a link here: https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6
  That link will provide you with all of the material you need to download to get osTicket up and running. Simply click the link and install the Web Platform Installer



</p>
<br /></p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
