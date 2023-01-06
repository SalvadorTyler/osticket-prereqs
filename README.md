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
- osTicket Installation files
- Heidi SQL

<h2>Installation Steps</h2>

<p>
</p>
<p>
Ok, so in this tutorial i will explain how to setup and install osticket a ticketing system. First we will have to create a Virtual machine using the Microsoft Azure portal. We are using a VM in order to protect our physical machine just in case something breaks.
  
 <img src="https://imgur.com/eQMK8y8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
<p>
</p>
<p>Set a name for your resouce group and virtual machine. next choose the size i recommend using 4 cpus and 16gb. Then you're gonna choose a username and passowrd after click review and create.
</p>
<img src="https://imgur.com/uBKE1EC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
</p>
<p>
next you're going to log into the new virtual machine, go to remote desktop, click on add pc and copy paste the ip address. Log in with the username and password you created earlier.
</p>  
<img src="https://imgur.com/Sh1Mjfa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
</p>
<p>
Now that you've logged in you're going to enable IIS by going to control panel and navigating to, uninstall a program, then click turn window features on or off on the left and side. and check the box next to internet information services, then click ok. 
</p>
<img src="https://imgur.com/6kTvgZE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>

</p>
<img src="https://imgur.com/qghGPBZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
</p>
<p>

</P>
<img src="https://imgur.com/38ODTQP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
<p>
</p>
<p>
</p>
<img src="https://imgur.com/3bJq2lC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<p>
</p>
<p>
</p>tiutaeughaliurghaleiughalrgn
<img src="https://imgur.com/qghGPBZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br /> 
<p>
</p>
<p>
</p>
<img src="https://imgur.com/wfaIL5A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<p>
</p>
<p>
</p>
<img src="https://imgur.com/4gOUn8l.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<p>
<p>Continue Setting up osticket in the browser MySQL Database: osTicket MySQL Username: root MySQL Password: Password1 Click “Install Now!”
Congratulations, hopefully it is installed with no errors!
Clean up
Delete: C:\inetpub\wwwroot\osTicket\setup
Set Permissions to “Read” only: C:\inetpub\wwwroot\osTicket\include\ost-config.php
Login to the osTicket Admin Panel (http://localhost/osTicket/scp/login.php)
<img src="https://imgur.com/mOAXRWu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
