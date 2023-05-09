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
In this tutorial i will explain how to setup and install osticket a ticketing system. First we will have to create a Virtual machine using the Microsoft Azure portal. We are using a VM in order to protect our physical machine just in case something breaks.
  
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
Now that you've logged in you're going to enable IIS by going to control panel and navigating to, uninstall a program, then click turn window features on or off on the left hand side. and check the box next to internet information services, then click ok. 
</p>
<img src="https://imgur.com/6kTvgZE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>

</p>
now that thats done you're going to go to this link https://drive.google.com/drive/u/1/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6 in here i've provided everything you'll need to download to get osticket up and running. for now we're going to download webplatforminstaller.
<img src="https://imgur.com/qghGPBZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
</p>
<p>

</P>
<br />
<p>
</p>
<p>
</p> next open  webplatforminstaller and in the search bar type in MySQL 5.5, click add, then search for php and add php 5.6.31, php 7.0.33 (x86), php 7.1.29 (x86), php 7.2.26 (x86), 7.3.25 (x86) then click install at the bottom
<img src="https://imgur.com/tfacBWM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<p>
</p>
<p>
</p> Afterwards you'll choose a password for MySQL make sure you remember this for later, then click continue and accept.
<img src="https://imgur.com/sGgQHcd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br /> 
<p>
</p>
<p>
</p> Now we are gonna go back doc from the link I provided and download PHPmanager, vcreditlist, and install them after. Then download osticket 1.15.8 from the doc, and extract the file. once you've done that open the osticket folder and copy the upload folder and paste it inside the C:\inetpub\wwwroot folder. Now you're gonna want to rename it to osTicket.
<img src="https://imgur.com/NTpRq2S.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<p>
</p>
<p>
</p> Ok now that we've done that we're gonna open IIS and click restart on the right hand side, Then navigate to sites on the left hand side, default web sitesand osticket. Now click browse .80 on the right side.
<img src="https://imgur.com/FqaRn1E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />


If done correctly it should take to a website that looks like this.
<p> <img src=https://imgur.com/3n6zxEL.png height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
  
<p> Once you've done that open phpmanager in IIS and click enable or disable an extension, Then enable php_intl.dll and php_opcache.dll and refresh the osticket site.
  
<p>
<img src="https://imgur.com/SzPkrMI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
  
 <p> Next you're going to go into file explorer and go to C:\inetpub\wwwroot\osticket\include and rename ost-sampleconfig.php to ost-config.php
    
<p>
<img src="https://imgur.com/l785aFd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
  Now right click on ost-config.php, go to properties, security, advanced, click disable inheritance. Remove all inherited permissions then click add, select a principle, type in everyone click ok then click full control and ok.
  
<p>
<img src="https://imgur.com/5NfHmEx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
  Ok now its time to setup osticket in the browser, fill out all the information necessary this can be whatever.
  
<p>
<img src="https://imgur.com/moYUTWX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
  
  When you get to MySQL database you'll download HeidiSQL from the download folder. Once you install HeidiSQL, launch it and click new, The password will be what you used for MySQL. Proceed to open, once open right click on unnamed and click create new and database, The name for the database will be osTicket. Once you've done that you can close out of that and type in osTicket in MqDQL databe on the osticket browser. now simply click install now
  
  
<p>
<img src="https://imgur.com/TNaQUlF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
  
  Just a few loose ends to clean up so now we will navigate to C:\inetpub\wwwwroot\osticket and delete setup. Then go to include\ost-config.php and reset the permissions to read  and read and execute only. 
  
  Congrats you've finished the installation process of osTicket. Now you can move on to osTicket: Post-Installation Configuration.
