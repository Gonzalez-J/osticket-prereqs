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

Welcome to my first tutorial!

First we will have to create a Virtual machine using the Microsoft Azure portal. We will be using a VM which is a remote computer. We are using a VM in order to protect our physical machine just in case something breaks. We will create a resource group and title it "osTicket". Afterwards creating a VM with 2-4 CPUs. In this example we will be using 4 CPUs.

<p>
<img src="https://i.imgur.com/DZyFdnX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next simply connect to your newly created VM (Virtual Machine) using RDC (Remote DesktopConnection) using the public IPv4 address. If you are a Mac user you will have to download Microsoft RDC.
<p>
<img src="https://i.imgur.com/5quNpxU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://imgur.com/a/NuvaxuZ" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

<h2>Installation Steps</h2>

Enable IIS (Internet Information Services)

Install  Web Platform Installer

Install MySQL

Set up User Name and Password

<p>
<img src="https://i.imgur.com/ERjyU6U.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>




<p>
<img src="https://i.imgur.com/LzWFrwz.png" width="80%" alt="Disk Sanitization Steps"/>
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

Furthermore, Now that we have enabled IIS we need to install Web Platform Installer. Here is a link: https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6
This link will provide you with all of the material needed to download osTicket and get it up and running. Simply click the link and install the Web Platform Installer, 

After installing Web Installer Platform, open it and install MySQL 5.5 from inside the application. Then install the x86 version of PHP up until 7.3. If you encounter any failed files such as C++ redistributable package as well as PHP 7.3.8 and PHP Manager for IIS, you can find those files with the install link.

</p>
<br /></p>
<p>
 Download osTicket and extract it. Copy the “upload” folder into c:\inetpub\wwwroot. Then rename the folder to osTicket.
 
Open IIS Manager and restart the server. Once inside IIS manager go to Sites->Default->osTicket on the right, click "Browse*.80" from there your default browser should open osTicket webserver.
  
<p>
<img src="https://i.imgur.com/APZgUTT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Assign permissions to ost-config.php Disable inheritance->Removeall
New Permissions->Everyone->all 
<p>
<img src="i.imgur.com/1nYaYGe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  
 
 To enable some extensions in IIS manager, go to Sites->Default->osTicket. Then double click on PHP manager and click on “Disable or enable an extension”. Enable “php_intl.dll” & “php_opcache.dll”. Then refresh the osTicket webserver and observe the changes. You should see that “Intl Extension” is now enabled.
<p>
<img src="https://i.imgur.com/1H0NzDU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

 Go back into c:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php rename the file to c:\inetpub\wwwroot\osTicket\include\ost-config.php
Assign permissions to ost-config.php Disable inheritance->Remove all
<p>
<img src="i.imgur.com/1nYaYGe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>  
  
 
 After setting up osTicket in the browser (click continue), you can name the Helpdesk to your liking and select a default email that will receive emails from customers who submit tickets.
  
<p>
<img src="i.imgur.com/1nYaYGe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 
 Continue Setting up osticket in the browser MySQL Database: osTicket MySQL Username: root MySQL Password: Password1 Click “Install Now!” Congratulations, hopefully it is installed with no errors! Clean up Delete: C:\inetpub\wwwroot\osTicket\setup Set Permissions to “Read” only: C:\inetpub\wwwroot\osTicket\include\ost-config.php Login to the osTicket Admin Panel (http://localhost/osTicket/scp/login.php)
 
 

