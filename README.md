<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Step 1. Setup Resources in Azure
- Step 2. Ensure Connectivity between the client and Domain Controller
- Step 3. 
- Step 4

<h2>Actions and Observations</h2>

<img width="1535" alt="Screen Shot 2024-05-19 at 6 30 45 PM" src="https://github.com/DereHz/azure-network-protocols/assets/169094076/b7f16b5a-b641-4380-86ea-1c1eb575b0b3">

Step 1. In Azure, Setup a Resource Groups 

<img width="1529" alt="Screen Shot 2024-05-19 at 6 31 35 PM" src="https://github.com/DereHz/azure-network-protocols/assets/169094076/6715bfb6-69ba-43d7-89c8-fc8cfed22568">
<img width="1536" alt="Screen Shot 2024-05-19 at 6 33 39 PM" src="https://github.com/DereHz/azure-network-protocols/assets/169094076/a21c9777-4d51-4c55-8362-602217c7733f">
<img width="1537" alt="Screen Shot 2024-05-19 at 6 34 21 PM" src="https://github.com/DereHz/azure-network-protocols/assets/169094076/74624ef3-bd75-46f2-8b7c-90959259fdff">
<img width="1536" alt="Screen Shot 2024-05-19 at 6 42 32 PM" src="https://github.com/DereHz/azure-network-protocols/assets/169094076/c36358e7-d71b-41cf-9f43-755b54534ed4">


Step 2. Create 2 Virtual Machines 
 - Create a Windows 10 Virtual Machine (VM)
 - While creating the VM, select the previously created Resource Group
 - While creating the VM, create a new Virtual Network (Vnet) 
 - Create a Linux (Ubuntu) Virtual Machine (VM)
 - While create the VM, select the previously created Resource Group and Vnet
 - Observe Your Virtual Network within Network Watcher

Note: Wait for the first VM to finish Deploying before creating the second VM. If not, the Vnet you created on the first VM wont show up when creating the second VM.

<img width="2306" alt="Screen Shot 2024-05-19 at 6 47 30 PM" src="https://github.com/DereHz/azure-network-protocols/assets/169094076/2d16cdc1-f2c4-416e-a7de-cabd1f1e8424">

Step 3. Open Microsoft Remote Desktop (If on Mac)
 - Click Add PC
 - for PC name, use VM-1's Public IP Address
 - Open the VM on the Microsoft Remote Desktop after adding the PC



Part 4. Install Software Within Windows 10 VM
 - Install and Open WireShark
 - Open PowerShell




















