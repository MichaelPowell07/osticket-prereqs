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
- Internet Information Services(IIS)
- Install PHP manager
- Install Rewrite Module
- Install VC File
- Install MYSQL File
- Install Heidid SQL
- osTicket v1.15.8
- Link to downloadshttps:[//drive.usercontent.google.com/download?id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD&export=download&authuser=0](url)
<h2>Installation Steps</h2>
1.) The first thing you are going to want to do is create a virtual machine by going to [https://portal.azure.com/#home](url) . Setup your virtual machine with Windows 10 Pro, version 22H2. You will want to create a virtual machine with at least 2vcpus and 16gbs of memory.

2.) Once you have created your virtual machine you will want to connect to it by using the public IP address the Virtual Machine (VM) is setup with. You will connect using the remote desktop connection app.      
![image](https://github.com/user-attachments/assets/dc480500-64eb-476d-92ea-32a177856004)
![image](https://github.com/user-attachments/assets/2499e8f8-29fe-46d5-879d-4cb8429b6786)





3.) Once you have connected to your virtual machine you will want to go to your control panel. from the control panel open up programs.Then select, turn windows features on and off.
![image](https://github.com/user-attachments/assets/e5a7c0ed-e971-4e97-b141-4e5b2e7581b3)

![image](https://github.com/user-attachments/assets/3649967f-d0a5-4d83-8f87-e8cad9f7e331)


4.) You will want to install/enable IIS in windows with CGI and common HTTP features 
World Wide Web services-> application development features -> [x] CGI [x] common HTTP features
![image](https://github.com/user-attachments/assets/cfc0df69-4c22-43f9-a9cb-0d096a394bb0)



Note make sure all common HTTP features are checked.
To make sure the IIS is installed/enabled go to a browser of your choice and search for 127.0.0.1 it should look something like this 
![image](https://github.com/user-attachments/assets/c24113df-453b-4e7b-8fda-ee5f490047fd)

5.) Now that the IIS is enabled, from the installation files, download and install PHP manager for IIS.
(PHPManagerforIIS_v1.5.0msi) Go through the install wizard and complete the install.

6.) Next from the Installation files, download and install the Rewrite Module (rewrite_amd64_en-US.msi)
