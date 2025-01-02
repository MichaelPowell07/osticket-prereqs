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
![image](https://github.com/user-attachments/assets/76cfcef6-a6ec-460a-a078-62725e258643)

7.) Create a folder in the C drive called PHP.

![image](https://github.com/user-attachments/assets/66b85363-3fab-4f16-86a8-f43667f74ecc)

8.) From the installation files, download PHP 7.3.8(php-7.3.88-nts-Win32-VC15-x866.zip) and unzip the contents into c:/PHP

![image](https://github.com/user-attachments/assets/a0e45c4f-b2e0-4b61-bccf-fc30182b9b16)

9.) Once you have downloaded and extracted the zip file into the PHP folder on the C drive, download and install the VC_redist.x86.exe from the installation files. Go through the setup wizard to finish setting up and installing the VC_redist.x86.exe.

![image](https://github.com/user-attachments/assets/e4b0ff58-df5e-4b2d-9c86-36deb22e083d)

10.) Download and install MYSQL 5.5.62(mysql-5.5.62-win32.msi) Run the setup wizard: Typical setup -> Launch configuration wizard (after install) -> standard configuration.

![image](https://github.com/user-attachments/assets/496dec5e-de66-4d05-b6ec-b94dab83e78d)

![image](https://github.com/user-attachments/assets/11e2879b-6171-417c-ab24-b334cfa99c17)

![image](https://github.com/user-attachments/assets/2014a848-2ec0-48a4-8d7e-ba1f4ccde9d7)

Make the new root password: Password1

![image](https://github.com/user-attachments/assets/a2f1806c-c9a7-4b90-970c-35aa6b9ebb80)

11.) Now that we have the files downloaded and installed we will want to search for the IIS in the windows search bar. Open IIS as an administrator.The program should look like this.

![image](https://github.com/user-attachments/assets/8d40bf3d-60fd-4138-9cbb-1d2041650bbf)

