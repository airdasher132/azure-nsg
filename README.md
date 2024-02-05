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

- Observe ICMP Traffic
- Configure NSG Rules
- Observe SSH Traffic on local VNET
- Observe DHCP Traffic

<h2>Actions and Observations</h2>

<p>

![image](https://github.com/airdasher132/azure-nsg/assets/158870278/ff978740-b066-46d1-b368-03804e6ff021)


</p>
<p>
This is using wire shark to observe different types of ICMP traffic that is coming through the virtual machine.
</p>
<br />

<p>

![image](https://github.com/airdasher132/azure-nsg/assets/158870278/7e62446f-9cfb-4952-9301-2696d83008d7)


</p>
<p>
I changed NSG rules on a seperate VM that is on the same VNet to block ICMP traffic and observe the results.
</p>
<br />

<p>

![image](https://github.com/airdasher132/azure-nsg/assets/158870278/6d5066a7-df6a-43d7-8105-07754ae8e5bb)


</p>
<p>
Using the command line to connect to the other VM through secure shell and filtering wireshark to display SSH traffic between the 2 machines.
</p>
<br />

<p>

![image](https://github.com/airdasher132/azure-nsg/assets/158870278/e6f5284b-2f65-4066-8447-be4a6a8c6ee1)

  
</p>
<p>
Finally showing how DHCP works when attempting to assign a new address or information to a VM.
</p>
