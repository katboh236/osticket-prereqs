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

- Created a Resource Group in Microsoft Azure 
- Created a Windows 10 Virtual Machine (VM) with 2-4 Virtual CPUs in Microsoft Azure
- Installed Microsoft Remote Desktop
- Connected to Virtual Machine (VM) with Remote Desktop
- Installed/Enabled Internet Information Services (IIS)
- Installed Web Platform Installer
- Installed MySQL 5.5 instead of username and password
- Installed PHP Version 7.3.8
- Installed PHP Manager 1.5.0 for IIS 10
- Installed C++ 2009 Redistributable Package
- Configured Permissions and Installed osTicket
- After-Installation Configuraton of osTicket

<h2>Installation Steps</h2>

<p>
<img src="https://imgur.com/PV6UpRw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Created Resource Group in Microsoft Azure - RG-osTicket in order to create Virtual Machine (VM).
</p>
<br />

<p>
<img src="https://imgur.com/yd5qvVP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://imgur.com/S0AwTNb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://imgur.com/w9j5OSV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Created a Windows 10 Virtual Machine (VM) with 2-4 Virtual CPUs in Microsoft Azure with standard D4s_v3 - 4 vcpus, 16 GiB memory size. Network interface: Virtual network - RG-osTicket-vnet; Subnet - 10.0.0.0/24; Public IP - VM-osTicket-ip.
</p>
<br />

<p>
<img src="https://imgur.com/lj7D0gm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://imgur.com/aWtaYZ2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://imgur.com/RHL4fo8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Installed Microsoft Remote Desktop and connected to Virtual Machine (VM) via Remote Desktop using public IP address.
</p>
<br />
<p>
<img src="https://imgur.com/aFxfQc3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
Installed/Enabled Internet Information Services (IIS) that created a web server on Virtual Machine (VM) to be used to serve up osTicket application.
</p>
<br />
<p>
<img src="https://imgur.com/IiRCvQQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://imgur.com/ZtvmG4o.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Installed Web Installer, instlled MySQL and added all versions of x86 PHP up until 7.3. Installed failed prerequisites: PHP Version 7.3.8, PHP Manager 1.5.0 for IIS 10 and Microsoft Visual C++ 2009 Redistributable Package.

</p>
<br />

<p>
<img src="https://imgur.com/4slP3kC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://imgur.com/IYCjrnj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Installed osTicket and enabled some extensions in IIS PHP Manager necessary for osTicket to function (php_imap.dll, php_intl.dll, php_opcache.dll).

</p>
<br />
<p>
<img src="https://imgur.com/C1YgYt6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://imgur.com/wDXEtLr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://imgur.com/tnTYPpY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Renamed ost-sampleconfig.php to ost-config.php (From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php To: C:\inetpub\wwwroot\osTicket\include\ost-config.php). Disabled all inherited permission for ost-config.php and assigned new permissions to "everyone".

</p>
<br />
