# Active-Directory-Lab
Basic Running Active Directory (Oracle VirtualBox)

# Overview
Based on Josh Madakor's tutorial: 

https://www.youtube.com/watch?v=MHsI8hJmggI

Project involves downloading and installing Oracle VirtualBox as our Virtual Machine, and using Windows 10 ISO and Server 2019 ISO to install two OS's on two seperate VM's. 

We will create our Domain Controller (DC) which will house the Active Directory. We will give this VM two network adapters (NIC), one will be used to connect to the internet and the other to connect to VirtualBox's private network. Once these are created, we will install Server 2019 onto our VM and assign IP addressing for our internal network. We will then install our Active Directory (Domain), configure NAT and Routing (in order to gain internet access through the DC), and set up a DHCP on the DC to automatically assign our machine with an IP address. Finally, we will run a PowerShell script that will autmoatically create 1,000 users. Another VM will be created which will connect to our DC.
