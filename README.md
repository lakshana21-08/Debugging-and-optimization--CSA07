**README – Cisco Packet Tracer Debugging & Optimization Tasks
Overview

This project demonstrates troubleshooting and optimization techniques in Cisco Packet Tracer using Smart Home, Fire Safety, and Smart Parking IoT networks. The tasks include network debugging, ARP table analysis, DHCP configuration, and ICMP packet analysis to ensure successful communication between devices.

Scenario 1 – Home Gateway IoT Network (Ping Debugging)
Objective
**
Identify the IoT device that is unreachable, correct its network configuration, and verify successful communication.

Steps
Open scenario1_STUDENT.pkt.
Switch to Simulation Mode.
Send a Simple PDU (Ping) from the Home Gateway or Smartphone to:
Door (IoT9)
Garage Door (IoT8)
Light (IoT6)
Lawn Sprinkler (IoT7)
Identify the device that fails.
Check its IP Address, Subnet Mask, and Default Gateway.
Correct the incorrect configuration.
Verify successful ping.
Open the Smart Home application and confirm the device is connected.
Control the device successfully.
Expected Result

All IoT devices respond successfully to ping and are accessible from the Smart Home application.

**Scenario 2 – ARP Table Analysis (Smart House Network)
Objective

Study how ARP maps IP addresses to MAC addresses and troubleshoot an unreachable IoT device.
**
Steps
Open Command Prompt on PC0 and execute:
arp -a
Execute the same command on Server1.
Observe existing ARP entries.
Ping each device individually:
Door (IoT2)
Window (IoT3)
Server1
Webcam (IoT4)
Webcam (IoT4(1))
Fan (IoT5)
After every successful ping, execute:
arp -a
Identify the device whose MAC address does not appear.
Check that device's IP configuration.
Correct the misconfiguration.
Repeat the ping test.
Expected Result

All devices respond successfully and their MAC addresses appear in the ARP table.

**Scenario 3 – Connect Server & Enable DHCP (Fire Safety Network)
Objective

Connect a new server and configure DHCP so all IoT devices receive IP addresses automatically.
**
Steps
Connect the Server to the Home Gateway or Switch using the correct copper cable.
Verify the link LEDs are green.
Assign the Server a static IP address.
Enable the DHCP service.
Create a DHCP Pool:
Default Gateway
Starting IP
Subnet Mask
DNS Server (optional)
Save the DHCP Pool.
Configure all IoT devices and Smartphone to obtain IP addresses using DHCP.
Renew the DHCP lease if required.
Verify each device receives a valid IP address.
Ping the Server and at least two IoT devices.
Verify active DHCP leases on the Server.
Expected Result

All devices receive valid IP addresses automatically and communicate successfully.

**Scenario 4 – PDU & ICMP Analysis (Smart Parking Network)
Objective

Analyze ICMP packets using Simulation Mode and troubleshoot communication failures.**

Steps
Open the Smart Parking topology.
Switch to Simulation Mode.
Send Simple PDUs from Laptop0 to:
Garage Door
RFID Reader
Motion Detector
Window
Identify successful and failed transmissions.
Select one successful PDU.
Examine each hop and verify:
ICMP Echo Request (Type 8)
ICMP Echo Reply (Type 0)
For the failed device:
Inspect packet flow.
Determine where communication stops.
Check IP configuration.
Correct the incorrect configuration.
Repeat the PDU test.
Expected Result

All devices respond successfully and ICMP Echo Request and Echo Reply packets are exchanged correctly.

Technologies Used
Cisco Packet Tracer
IPv4 Addressing
Home Gateway
DHCP
ARP (Address Resolution Protocol)
ICMP (Ping)
IoT Devices
Simulation Mode
Smart Home Network
Fire Safety Network
Smart Parking Network
Learning Outcomes
Configure and troubleshoot IoT devices.
Analyze ARP tables.
Configure DHCP services.
Debug IP addressing issues.
Understand ICMP packet flow.
Use Simulation Mode for network analysis.
Verify successful network communication.
Conclusion

This project provides hands-on experience in debugging and optimizing IoT networks using Cisco Packet Tracer. By analyzing ARP tables, configuring DHCP services, troubleshooting IP addressing issues, and examining ICMP packet exchanges, reliable communication between all network devices is achieved while reinforcing fundamental networking concepts.
