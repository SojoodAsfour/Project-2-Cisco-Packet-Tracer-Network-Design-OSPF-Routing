# 🌐 ENCS3320 – Project #2  
## Cisco Packet Tracer Network Design & OSPF Routing

---

## 📌 Project Overview

This project focuses on designing and implementing a **multi-area routed network** using **Cisco Packet Tracer**.

The topology consists of:

- 🏫 Central Campus Network (Area 0)
- 🌍 West Network (Area 20)
- 🌎 East Network (Area 30)
- 🌐 ISP Network

The project integrates:

- IP Subnetting
- Static IP configuration
- Wireless LAN configuration
- OSPF routing (multi-area)
- Network testing and troubleshooting

---

## 🎯 Objectives

- Design an IP addressing scheme using subnetting 🧮  
- Configure routers and switches in Cisco Packet Tracer 🔧  
- Implement OSPF multi-area routing 🔁  
- Configure WLAN using WPA2 security 🔐  
- Test connectivity using ping and tracert 📡  
- Develop professional technical documentation 📄  

---


---

## 🧮 IP Subnetting Task

Main IP format:
1X.Y.128.0/17

Where:
- X and Y = last four digits of team leader SID

Example:
If SID = 1237090  
→ X = 70  
→ Y = 90  
→ Network = 170.90.128.0/17

Each subnetwork was calculated based on the number of required hosts.

The report includes:
- Network address
- Broadcast address
- Usable range
- CIDR notation

---

## 🏗️ Network Topology

The topology includes:

### 🏫 Central Campus (Area 0)
- 2 Routers
- 1 Switch
- 1 PC
- 1 Laptop
- Static IP configuration

---

### 🌍 West Network (Area 20)
Subnets:
- West LAN1
- West LAN2
- West WLAN

Devices:
- 3 Routers
- 2 Switches
- 1 Access Point
- PCs & Laptops
- Smartphone

Wireless Configuration:
- SSID: ENCS3320WestSTName
- Security: WPA2 Personal
- Encryption: AES
- Key: ST_#

---

### 🌎 East Network (Area 30)
Subnets:
- East LAN1
- East LAN2
- East WLAN

Devices:
- 3 Routers
- 2 Switches
- 1 Access Point
- PCs & Laptops
- Smartphone

Wireless Configuration:
- SSID: ENCS3320EastSTName
- Security: WPA2 Personal
- Encryption: AES
- Key: ST_#

---

### 🌐 ISP Network
- 1 Router
- OSPF enabled

---

## 🔁 Routing Configuration (OSPF)

All routers are configured using:

```bash
Router(config)# router ospf 1
Router(config-router)# network <ID-Address> <WildCard-Mask> area <Area-ID>


