# Active-Directory-Lab
Basic Running Active Directory (Oracle VirtualBox)

# Overview
Based on Josh Madakor's tutorial: 

https://www.youtube.com/watch?v=MHsI8hJmggI

Project involves downloading and installing Oracle VirtualBox as our Virtual Machine, and using Windows 10 ISO and Server 2019 ISO to install two OS's on two seperate VM's. 

We will create our Domain Controller (DC) which will house the Active Directory. We will give this VM two network adapters (NIC), one will be used to connect to the internet and the other to connect to VirtualBox's private network. Once these are created, we will install Server 2019 onto our VM and assign IP addressing for our internal network. We will then install our Active Directory (Domain), configure NAT and Routing (in order to gain internet access through the DC), and set up a DHCP on the DC to automatically assign our machine with an IP address. Finally, we will run a PowerShell script that will autmoatically create 1,000 users. Another VM will be created which will connect to our DC.

# Setup

Install Oracle VM VirtualBox as well as the Extension Pack: https://www.virtualbox.org/wiki/Downloads

In order to install Windows 10 and Windows Server 2019 into VirtualBox, we need their respective ISO files:

Windows 10 (64-bit ISO): https://www.microsoft.com/en-us/software-download/windows10ISO

Server 2019 (ISO): https://www.microsoft.com/en-us/evalcenter/download-windows-server-2019

In VirtualBox, create a VM named "DC" (Domain Control):
<img width="1230" alt="Screenshot 2024-09-28 at 4 29 27 PM" src="https://github.com/user-attachments/assets/f199e3cb-9249-401c-bd12-81ad11f858f9">
Make sure to allocate an appropriate memory and cores:
<img width="1233" alt="Screenshot 2024-09-28 at 4 29 57 PM" src="https://github.com/user-attachments/assets/cb07e1aa-fa20-4e88-8ce1-03e00054ec3f">
<img width="955" alt="Screenshot 2024-09-28 at 4 30 12 PM" src="https://github.com/user-attachments/assets/5a1f750f-2165-4cd7-8063-607b802aded1">

Make sure you have one NIC dedicated to internet that will be running NAT:
<img width="950" alt="Screenshot 2024-09-28 at 4 21 48 PM" src="https://github.com/user-attachments/assets/caf5bb8d-078d-469c-a44e-fe6e7f2a8097">
Add an Internal Network adapter (private network):
<img width="951" alt="Screenshot 2024-09-28 at 4 22 15 PM" src="https://github.com/user-attachments/assets/66bc7961-4dee-40a1-914f-c8fed7bda78d">





