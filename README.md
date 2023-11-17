


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
These are the steps to be taken to implement the processs of installation of osTicket.
1. On our web browser we visit www.portal.azure.com. We create a resource group and give it any name of our choosing, after this is done we proceeed to create the Azure virtual Machine, the virtual machine will have to be created with at least 2Vcpu and a memory of 16gb.
2. Once the virtual machine has been created we would establish connection between the Virtual machine and Remote desktop connection by getting the IP address of virtual machine just created and pasting into the remote network connection. 
![Capture](https://github.com/eyekay2518/osticket-prereqs/assets/67752659/13229f34-cc03-4fa8-b7a7-598b67f0ebd5)
3.Install and enable IIS: From the control panel in the virtual machine, we search Programs,then on the programs and features options we click on turn windows features off or on. On the turn windows features OFF or ON, we check all the required options in the checkbox, this include internet information services, world wide web services,application development features,CGI, common HTTP features. To ensure that IIS is enabled/installed on our virtual machine, we input the ip address 127.0.0.1, this ensures that the computer connects and communicates with itself.
![Capture3](https://github.com/eyekay2518/osticket-prereqs/assets/67752659/6f173f1e-a7d4-4192-aafd-94b989e5f6c7)
4. Download and install PHP Manager for IIS
![Capture4-php manager for IIS](https://github.com/eyekay2518/osticket-prereqs/assets/67752659/1540d761-1083-47fa-9660-f07917fe2e12)
5. From the installation files,we download and install the IIS URL rewrite module
![Capture5-IIS Url Rewrite Module](https://github.com/eyekay2518/osticket-prereqs/assets/67752659/d2f1c3e0-75e8-480b-972c-efcfa632d6af)
6. ON the virtual machine, go to windows(C) and create a folder, we name the folder PHP
7. We then proceed to download and install PHP 7.3.8, after download is done extract all content of the just downloaded file to C:\PHP
8. Download and install VC.redistX8.exe
![vc redistx86](https://github.com/eyekay2518/osticket-prereqs/assets/67752659/2acc25ba-74ed-4e29-a304-6b1b2d685f1b)
Download and install MySQL 5.5.62
![Capture7a-MySQL Installation](https://github.com/eyekay2518/osticket-prereqs/assets/67752659/5d3d807b-1c59-4a2e-9c8c-7a6ea2d43c55)
After the installation of MySQL, we proceed to  setup the MySQL server instance configuration wizard
![Capture7b-MySQL Standard Config Wizard](https://github.com/eyekay2518/osticket-prereqs/assets/67752659/354bcfd5-b165-4bf6-b74e-222433aca8d7)
we click on standard configuration,set up password of our choice.
![Capture7c-MySQL Password](https://github.com/eyekay2518/osticket-prereqs/assets/67752659/82fce911-bf6d-4e1e-a32b-a0c7905de505)
Then execute and finish
![Capture7-MySQL install](https://github.com/eyekay2518/osticket-prereqs/assets/67752659/a71b3aba-ef4f-48e7-ade2-8c2222329668)














<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
