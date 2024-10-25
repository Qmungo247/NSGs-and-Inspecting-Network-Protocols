# NSGs-and-Inspecting-Network-Protocols


<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>Walkthrough</h2>

<p>

![Screenshot 2024-10-25 161610](https://github.com/user-attachments/assets/3b69a3a5-9e6e-4fae-8ff3-5a55639baac2)

</p>
<p>
Create 2 VM's in Azure. One running Windows & the other running Linux. Then grab the privite IP of the Windows VM And Remote Desktop Connect to it.

</p>
<br />

<p>

  ![Screenshot 2024-10-25 150455](https://github.com/user-attachments/assets/035ae20e-7dc3-4d5b-9d84-b3b076189adb)

</p>
<p>
Once Connected to the Windows VM. Download & install Wireshark. (Windows x64 Installer) This allows you to view traffic between the 2 VMS.
</p>
<br />

<p>

![Screenshot 2024-10-25 162906](https://github.com/user-attachments/assets/66ede834-0087-4816-b7e4-a7308784b4ad)

</p>
<p>
After wireshark is installed. Open the app select ethernet interface & start a package Capture & observe the traffic. 

</p>
<br />

![image](https://github.com/user-attachments/assets/be095fd3-184c-4efb-bf31-93f1b1feaeff)

</p>
<br />

Filter ICMP traffic on wireshark & grab the Linux Private IP address from azure. Run Power Shell on the Windows VM & Ping the Linux VM Private IP address. Observe the trafffic in Wireshark. Ping is used for testing network connectivity by sending packets of data and measuring the response time.


