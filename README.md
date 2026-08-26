# **Cisco Packet Tracer — Small Office Business Network**

## 

# **Project 1 Overview**

# 

# This project demonstrates the design, configuration, testing and troubleshooting of a simulated small-office Local Area Network using Cisco Packet Tracer.

# 

# The lab was created to develop practical networking skills relevant to entry-level IT Support, Service Desk, Network Support and Cloud Support roles.









# 

# **Business Scenario**

# 

# **ZentrixLabs Solutions Ltd** requires a small office network supporting two business departments:

# 

# \- Finance

# \- Operations

# 

# The network must allow all workstations to communicate across the LAN and access a shared network printer.

# 







# **Network Topology**

# 

# "Small Office Network Topology" (Screenshots/network-topology.png)

# 

# The completed topology contains:

# 

# \- 1 Cisco router

# \- 2 Cisco switches

# \- 6 workstations

# \- 1 shared network printer

# \- Finance and Operations departments





# 



# **IPv4 Addressing**

# 

## **The network uses:**

# 

# "192.168.10.0/24"

# 

## **Subnet Mask:** "255.255.255.0"

# 

## **Default Gateway:** "192.168.10.1"

# 

# **Device        | IPv4 Address | Default Gateway**

# R1 G0/0       | 192.168.10.1 | N/A

# FIN-PC01      | 192.168.10.11| 192.168.10.1

# FIN-PC02      | 192.168.10.12| 192.168.10.1

# FIN-PC03      | 192.168.10.13| 192.168.10.1

# OPS-PC01      | 192.168.10.21| 192.168.10.1

# OPS-PC02      | 192.168.10.22| 192.168.10.1

# OPS-PC03      | 192.168.10.23| 192.168.10.1

# Office Printer| 192.168.10.50| 192.168.10.1

# 

# All end devices use static IPv4 addressing.

# 







# **Technologies and Concepts**

# 

# \- Cisco Packet Tracer

# \- Cisco IOS

# \- Ethernet

# \- IPv4

# \- "/24" subnetting

# \- Default gateways

# \- Static addressing

# \- Switching

# \- Router interfaces

# \- ARP

# \- ICMP

# \- LAN connectivity testing

# \- Structured troubleshooting

# 









# **Router Configuration Verification**

# 

# The router interface was verified using:

# 

# show ip interface brief

# 

# "Router Interface Status" (Screenshots/router-interface-status.png)

# 

# The output confirms that "GigabitEthernet0/0" is configured as:

# 

# 192.168.10.1

# 

# and is operating in an:

# 

# up/up

# 

# state.







# 

# **Gateway Connectivity Test**

# 

# "Gateway Ping Test" (Screenshots/gateway-ping.png)

# 

# A workstation successfully pinged the default gateway at:

# 

# 192.168.10.1

# 

# The successful ICMP replies confirmed connectivity between the workstation and router.









# 

# **Shared Printer Connectivity Test**

# 

# "Printer Ping Test" (Screenshots/printer-ping.png)

# 

# A workstation successfully communicated with the shared network printer at:

# 

# 192.168.10.50

# 

# This verified end-device-to-printer connectivity across the LAN.









# 



# **Cross-Switch Connectivity**

# 



# "Cross-Switch Ping Test" (Screenshots/cross-switch-ping.png)

# 

# A workstation connected to one switch successfully communicated with a workstation connected to the second switch.

# 

# This verified connectivity across the path:

# 

# Finance PC

# &#x20;   |

# &#x20;  SW1

# &#x20;   |

# &#x20;  SW2

# &#x20;   |

# Operations PC

# 

# and demonstrated successful Layer 2 communication between the two parts of the network.









# 



# **Troubleshooting Exercise**

# 

# A workstation was intentionally configured with an incorrect IPv4 address/subnet configuration to simulate a realistic support incident.

# 



## **Before Remediation**

# 

# "Incorrect IP Configuration" (Screenshots/ip-fault-before.png)

# 

# The incorrect addressing configuration prevented normal network communication.

# 

# The fault was investigated by checking:

# 

# \- IPv4 address

# \- Subnet mask

# \- Default gateway

# \- Expected network range

# 





## **After Remediation**

# 

# "Corrected IP Configuration" (Screenshots/ip-fault-after.png)

# 

# The incorrect configuration was corrected and connectivity was successfully restored.

# 

# This exercise demonstrated a basic troubleshooting methodology:

# 

# Identify the problem

# &#x20;       ↓

# Inspect configuration

# &#x20;       ↓

# Identify incorrect setting

# &#x20;       ↓

# Correct configuration

# &#x20;       ↓

# Retest connectivity

# &#x20;       ↓

# Confirm resolution.











# 

# **ICMP Simulation Mode**

# 

# "ICMP Simulation" (Screenshots/icmp-simulation.png)

# 

# Cisco Packet Tracer Simulation Mode was used to observe network traffic and follow ICMP communication between devices.

# 

# This helped demonstrate the relationship between packet-level communication and the physical/logical network topology.

# 









# **Verification Performed**

# 

# The completed network was tested using:

# 

# ping

# ipconfig

# arp -a

# show ip interface brief

# 

# Testing confirmed:

# 

# \- Router interface operational

# \- Default gateway reachable

# \- Shared printer reachable

# \- Finance-to-Operations connectivity

# \- Cross-switch communication

# \- Successful ICMP Echo Request/Reply traffic

# \- Connectivity restored after troubleshooting

# 







# **Skills Demonstrated**

# 

# This project demonstrates practical experience with:

# 

# \- Small-office network design

# \- Cisco Packet Tracer

# \- Cisco IOS commands

# \- IPv4 addressing

# \- Subnet masks

# \- Default gateways

# \- Static host configuration

# \- Ethernet switching

# \- Router interface configuration

# \- ICMP connectivity testing

# \- ARP fundamentals

# \- Cross-switch communication

# \- Fault identification

# \- IP configuration troubleshooting

# \- Verification after remediation

# \- Technical documentation

# \- Git and GitHub project documentation

# 









# **Project Files**

# 

# packet-tracer-small-office-network/

# │

# ├── README.md

# ├── .gitignore

# ├── ZentrixLabs-Small-Office-Network.pkt

# │

# └── Screenshots/

# &#x20;   ├── network-topology.png

# &#x20;   ├── router-interface-status.png

# &#x20;   ├── show-ip-interface-brief.png

# &#x20;   ├── gateway-ping.png

# &#x20;   ├── printer-ping.png

# &#x20;   ├── cross-switch-ping.png

# &#x20;   ├── ip-fault-before.png

# &#x20;   ├── ip-fault-after.png

# &#x20;   └── icmp-simulation.png

# 





# **Outcomes**

# 

# The final network successfully provides connectivity between Finance and Operations workstations, the router and the shared office printer.

# 

# The project also demonstrates the ability to identify and correct an IPv4 configuration fault and verify the resolution using structured connectivity testing.

# 

# \---

# 

# **Project 1 of a six-project Cisco Packet Tracer networking portfolio.**

