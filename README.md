


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
Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine
- Internet Information Services(IIS)
- PHP Manager for IIS
- Rewrite Module
- PHP 7.3.8
- VC redistX86
- MySQL 5.5.62
- osTicket V1.15.8
- Heidi SQL
- Links to download :https://docs.google.com/document/d/12QH7yrsaiUfYNOgZK7KgTSZQSJ-HYTSVcGFildWMRig/edit#bookmark=id.cajb4ktub1km

<h2>Installation Steps</h2>
<h3>These are the steps to be taken to implement the processs of installation of osTicket.</h3>
<p>
1. On our web browser we visit https://portal.azure.com. We create a resource group and give it any name of our choosing, after this is done we proceeed to create the Azure virtual Machine, the virtual machine will have to be created with at least 2 Virtual cpu and a memory of 16gb.</p>
<p>
2. Once the virtual machine has been created we would establish connection between the Virtual machine and Remote desktop connection by getting the IP address of virtual machine just created and pasting into the remote network connection. </p>
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/04daab5e-8fcc-4f5a-bdbc-fd4a011fd131"
height="50%" width="50%" alt="remote desktop">
<br>
<br>
<p>
3. Install and enable IIS: From the control panel in the virtual machine, we search Programs,then on the programs and features options we click on turn windows features off or on. On the turn windows features OFF or ON, we check all the required options in the checkbox, this include internet information services, world wide web services,application development features,CGI, common HTTP features. To ensure that IIS is enabled/installed on our virtual machine, we input the ip address 127.0.0.1, this ensures that the computer connects and communicates with itself.
</p>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/6f173f1e-a7d4-4192-aafd-94b989e5f6c7" 
  height="50%" width="100%" alt="disk sanitization step"/>
  <br>
  <br>
  
<p>  4. Download and install PHP Manager for IIS</p>
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/1540d761-1083-47fa-9660-f07917fe2e12"
  height="50%" width="50%" alt="disk sanitization step"/>
  <br>

<p>  5. From the installation files,we download and install the IIS URL rewrite module</p>
<br>
 <img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/d2f1c3e0-75e8-480b-972c-efcfa632d6af"
  height="50%" width="50%" alt="disk sanitization step"/>
  <br>
<p>  6. ON the virtual machine, go to windows(C) and create a folder, we name the folder PHP</p>
<br>
<p>  7. We then proceed to download and install PHP 7.3.8, after download is done extract all content of the just downloaded file to C:\PHP</p>
<p>  8. Download and install VC.redistX8.exe</p>
<br>
 <img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/2acc25ba-74ed-4e29-a304-6b1b2d685f1b"
  height="50%" width="50%" alt="disk sanitization step"/> 
  <br>
  <br>
<p>  9.Download and install MySQL 5.5.62</p>
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/5d3d807b-1c59-4a2e-9c8c-7a6ea2d43c55"
  height="50%" width="50%" alt="disk sanitization step"/> 
  <br>
<p>  10.After the installation of MySQL, we proceed to  setup the MySQL server instance configuration wizard</p>
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/354bcfd5-b165-4bf6-b74e-222433aca8d7"
height="50%" width="50%" alt="disk sanitization step"/> 
<br>
<p>  11.we click on standard configuration,set up password of our choice.</p>
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/82fce911-bf6d-4e1e-a32b-a0c7905de505"
height="50%" width="50%" alt="disk sanitization step"/>
<br>
Then execute and finish
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/a71b3aba-ef4f-48e7-ade2-8c2222329668"
height="50%" width="50%" alt="disk sanitization step"/> 
<br>
<br>
<p>  12.Open the previously installed IIS, register PHP by clicking on the PHP manager icon, and follow all necessary path. 
Reload IIS by stopping and restarting the server.</p>
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/11931156-a33d-4f7d-8b05-a96042decc78"
height="50%" width="50%" alt="disk sanitization step"/> 
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/5371c098-1d9c-4704-bba5-7b0289fba091"
height="50%" width="50%" alt="disk sanitization step"/> 
<p>  13.Download and install osticket from the Installation files
From the just downloaded osTicket, we move the folder called "upload" to the windows(C)folder called inetpub. In inetpub, we move folder to another folder called wwwroot</p>
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/d1c8a57d-54d7-462b-94ae-42eed2cf41e7"
  height="50%" width="50%" alt="disk sanitization step"/> 
  <br>
<p>  14.Rename the folder called UPLOAD to osticket</p>
<p>  15.We then reload IIS by stopping and restarting
From IIS, we go to sites,then default, osticket, on the right we click on Browse *80 (http)</p>
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/d3690681-c50d-4904-a13d-9a3c1afba3fb"
height="50%" width="50%" alt="disk sanitization step"/> 
<br>
<p>  16.By clicking on Browse *80, it takes us to the osticket installer URL, we see some extensions are not enabled</p>
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/5eb02590-bda4-408a-8d0e-409d15b83eb2"
height="50%" width="50%" alt="disk sanitization step"/>
<br>
<p>  17.To enable extensions, click PHP manager,then we go to enable or disable extension. We then enable the following extension
<ol>
  <li>php-imap.dll</li>
  <li>php-itl.dll</li>
  <li>php-opcache</li>
</ol>
Refresh and notice the changes</p>
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/26b07091-6f9c-4fdf-a3e4-9fb68a10cb2b"
height="50%" width="50%" alt="disk sanitization step"/> 
<br>
<p>  18.From the osticket installation folder, we rename folder called ost-sampleconfig.php to ost-config.php.This is done by clicking on  the windows(C) folder,click on inetpub,then wwwroot,then osticket, we click on file called include,then on  the ost-sampleconfig.php file we rename to ost-config.php.</p>
<br>
<p>We have to assign permission to the just renamed  ostconfig.php file. 
To do that, from the windows(C) file click on inetpub,followed by wwwroot,then osticket,click on the include file, then from the ost-config.php file,right click to open properties ,then click on security, then advanced </p>
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/a878f865-d88e-4156-9f49-b9e2190dad1c"
height="50%" width="50%" alt="disk sanitization step"/>
<br>
<p>  19.Continue setting up osticket in browser,click continue, then enter your preferred  helpdesk name and email under the helpdesk URL.</p>
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/7b21aff9-1f2f-43b6-a96f-0509499de8d0"
height="50%" width="50%" alt="disk sanitization step"/> 
<br>
<p>  20.From the installation file, download and install Heidi SQL
<ol>
<li>open Heidi SQL</li>
<li>Create a new session with the following credentail detail</li>
<li>User: root </li>
<li>Password:Password1</li>
</ol>
</p>
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/ee30c716-ed9b-40de-b74e-eb8ed67154d3"
height="50%" width="50%" alt="disk sanitization step"/> 
<br>
<p>  21.After this is done, we connect to the session, and create a database called osticket</p>
<br>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/45d76ae2-7519-4be8-b38a-c0f1f4ed5e74"
height="50%" width="50%" alt="disk sanitization step"/> 
<br>
<p>  22.Finish up installation of osticket
<ol>
  <li>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/e13c3435-7f8b-4b57-ac7c-dc54a8bf5b02"
height="50%" width="50%" alt="disk sanitization step"/> </li>
  <br>
  <li>
<img src="https://github.com/eyekay2518/osticket-prereqs/assets/67752659/3d81fa48-14a7-45fd-81a8-102cbfb906f4"
height="50%" width="50%" alt="disk sanitization step"/> </li>
</ol>
</p>
<p>CleanUp:
Delete the setup folder inside your osticket folder by clicking on the (C) folder,then inetpub,then wwwroot,then osticket,in the osticket folder we click on the setup file to delete.</p>


























