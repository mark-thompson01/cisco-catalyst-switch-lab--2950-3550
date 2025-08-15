# cisco-catalyst-switch-lab--2950-3550

# 🖧 Cisco Catalyst Switch Lab - 2950-3550

This repository contains my **hands-on lab using a Cisco Catalyst 2950 and 3550 switch**, demonstrating foundational switch management and configuration skills.  

While the creation of VLANs and setting up Trunking is demonstrated. This lab is more focused on layer 2 switching. Inter-VLAN routing is not implemented in this setup due to a single available subnet.

These are fairly older models, but serve as a great tool for practicing networking fundamentals.

![Cisco Catalyst 2950](Images/Switches.jpg)



---


## 📖 Overview

This lab walks through the full process of connecting to, factory resetting, configuring, and managing a **Cisco Catalyst 2950 and 3550 switch** using the CLI via PuTTY Terminal Emulator.  

It covers console connectivity, factory resets, switch setup from scratch, VLAN management, port security, monitoring via SPAN, Spanning Tree Protocol - STP and Trunk port configuration.


---


## 🗂 Lab Demonstrations

  - Connecting to the Switch
  - Performing a Factory Reset
  - Configuring the Swtich from Scratch
  - Post Initial Setup
  - VLAN Creation and Managment
  - Port Security
  - SPAN - Switch Port Analyzer Configuration
  - Trunk Configuration
  - Spanning Tree Protocol (STP) Root Bridge Configuration


---


Key topics include:
- VLAN creation and port assignment
- Trunk configuration with a hardened native VLAN
- Spanning Tree Protocol (STP) root bridge configuration
- SPAN (port mirroring) for traffic analysis

> **Note:** Due to lab constraints, all devices operate within a single IP subnet. Inter-VLAN routing is not demonstrated in this setup.



---


🖥️ **Live Project Webpages:**  
👉 [Cisco Catalyst Switch Lab 1](https://mark-thompson01.github.io/MTPortfolio/Skills/Labbing%20with%20a%20Cisco%20Catalyst%202950%20Switch/)

👉 [Cisco Catalyst Switch Lab 2](https://mark-thompson01.github.io/MTPortfolio/Skills/Cisco%20STP%20Trunking%20Lab/)


---


## Topology
**Switch 1:** Cisco Catalyst 2950 (Layer 2) – VLAN creation, access port assignments, SPAN configuration
**Switch 2:** Cisco Catalyst 3550 (Layer 3-capable) – Trunking, STP root bridge

**VLAN Plan:**
| VLAN ID | Name   | Purpose         |
|---------|--------|-----------------|
| 1       | native | Management      |
| 10      | Lab-2  | Experiment      |
| 20      | Lab-2  | Workstations    |
| 99      | Native | Native VLAN for trunk |

---

## Key Commands for Verification
```bash
show vlan brief
show interfaces trunk
show spanning-tree vlan 10
show spanning-tree vlan 20
show monitor session 1
```

---


## 🎯 Purpose

The purpose of this lab is to:

- Gain hands-on experience configuring and managing a **Cisco Catalyst switch**  
- Learn and practice:
  - Basic switch setup
  - VLAN creation and port assignments
  - Securing access via passwords and port security
  - Using SPAN (port mirroring) to capture and analyze traffic
- Build familiarity with the **Cisco IOS CLI**, a critical skill for networking and CCNA studies.


---


## 🛠️ Tech Used

- Cisco Catalyst 2950 and 3550 managed switches
- DB9 serial to console port cable
- PuTTY terminal emulator
- Windows Desktop
- Wireshark


---


## 📁 More from Me

Visit my full GitHub Pages portfolio to explore additional projects:

🔗 [MTPortfolio – Full Project Index](https://mark-thompson01.github.io/MTPortfolio/)


---


📄 **License**  
This content is licensed under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)






