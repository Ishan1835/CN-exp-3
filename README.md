#CN-3
Router Configuration Experiment
This repository contains the steps and configuration details for a network experiment involving a router and two PCs. The objective is to demonstrate the configuration of IP addresses in a router to establish both physical and logical connectivity between the devices. 🧑‍💻

📋 Prerequisites
Before starting, ensure you are familiar with the following concepts:

IP Address: A numerical label assigned to each device connected to a computer network.

Range of IP Address: The set of IP addresses that can be assigned within a specific network.

Classes of IP Address: The classification system for IP addresses (e.g., Class A, B, C).

💻 Components
The experiment requires the following components:

Devices	Required Number
PCs	2
Router	1
Copper cross-over cables	2

Export to Sheets
🗺️ Addressing Table
The following IP addressing scheme is used for the network configuration:

Device	Interface	IP Address	Subnet Mask	Gateway
PC0	Fa0/0	192.168.10.2	255.255.255.0	192.168.10.1
PC1	Fa0/0	192.168.11.2	255.255.255.0	192.168.11.1
Router0	GigabitEthernet0/0	192.168.10.1	255.255.255.0	
Router0	GigabitEthernet0/1	192.168.11.1	255.255.255.0	

Export to Sheets
🛠️ Procedure
The experiment is conducted using Cisco Packet Tracer and involves the following steps:

Step 1: Initial Setup
Drag a router and two PCs into the console area of Cisco Packet Tracer.

Step 2: Physical Connection
Select the 

Copper cross-over cable from the connectivity options.

Click on 

PC0 and select interface Fa0/0.

Click on 

Router0 and select interface GigabitEthernet0/0.

This connects 

PC0 to Router0.

Again, select the 

Copper cross-over cable.

Click on 

Router0 and select interface GigabitEthernet0/1.

Click on 

PC1 and select interface Fa0/0.

This establishes the physical connections between the PCs and the router.

Step 3: Logical Configuration
PC0 Configuration
Click on 

PC0 and go to the Config tab.

Select 

FastEthernet0/0 in the left pane.

Configure the IP Address as 

192.168.10.2 and Subnet Mask as 255.255.255.0.

Navigate to the 

Settings tab and set the Default Gateway to 192.168.10.1.

PC1 Configuration
Repeat the same procedure for 

PC1.

Configure the IP Address as 

192.168.11.2 and Subnet Mask as 255.255.255.0.

Navigate to the 

Settings tab and set the Default Gateway to 192.168.11.1.

Router0 Configuration
Click on 

Router0 and select the Config tab.

Select 

GigabitEthernet0/0 and configure the IP Address as 192.168.10.1 and Subnet Mask as 255.255.255.0.

Select 

GigabitEthernet0/1 and configure the IP Address as 192.168.11.1 and Subnet Mask as 255.255.255.0.

Step 4: Verifying Connectivity
To check if the PCs are logically connected, click on 

PC1.

Go to the 

Desktop tab and click on the Command Prompt icon.

Type the command 

ping 192.168.10.2 to check for a successful connection to PC0
