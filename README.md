Networkwalks Cybersecurity Internship — Week 2

Footprinting, Reconnaissance & Network Scanning

**Batch:** B083  
**Participant:** Dan Ngechu  
**Date:** 18 September 2026  
**Program:** Networkwalks Cybersecurity Internship


Overview

Week 2 focused on practical cybersecurity reconnaissance and network-scanning activities. The exercises covered passive information gathering, footprinting, Google Hacking Database (GHDB) techniques, Maltego-based reconnaissance, theHarvester, and network discovery using Zenmap.

The practical work was performed within the scope defined by the Networkwalks Week 2 project modules, using the specified targets and locally authorized network environment where applicable.


Week 2 Modules

PM1 — Footprinting with Multiple Kali Tools

Tools used:

- WHOIS
- WhatWeb
- nslookup
- cURL
- wafw00f
- DNSRecon

**Target:** `networkwalks.com`

The module focused on gathering publicly available information about the target domain using multiple reconnaissance tools.


PM2 — Footprinting with GHDB

The Google Hacking Database (GHDB) module involved researching publicly indexed resources using Google dorks.

Activities included:

- Security-camera-related search queries
- Publicly indexed mathematics PDF directories

The exercise demonstrated how search engines can expose information that has been indexed publicly.


PM3 — Footprinting with Maltego

**Target:** `networkwalks.com`

Maltego Graph was used to create a Domain entity for the target and perform email-related reconnaissance transforms.

Activities included:

- Creating a Domain entity
- Configuring `networkwalks.com`
- Running an email search-engine transform
- Running an email extraction transform using existing entity properties
- Recording the resulting transform output


PM4 — Footprinting with theHarvester

**Target:** `microsoft.com`

Two reconnaissance activities were performed:

1. theHarvester using the Baidu source with a result limit of 1000.
2. theHarvester using all available sources with a result limit of 50.

The available sources and resulting information varied according to the current configuration and availability of external services.


PM5 — Network Scanning with Zenmap

**Target subnet:** `192.168.1.0/24`

Zenmap was used to perform a ping scan of the local network.

The scan identified:

- 4 live hosts
- IP addresses of the discovered hosts
- MAC addresses where available
- A network topology representation


Tools & Technologies

| Tool | Purpose |
|---|---|
| Kali Linux | Cybersecurity testing and reconnaissance environment |
| WHOIS | Domain registration information |
| WhatWeb | Web technology identification |
| nslookup | DNS information gathering |
| cURL | HTTP response/header inspection |
| wafw00f | Web Application Firewall identification |
| DNSRecon | DNS enumeration |
| Google / GHDB | Search-engine-based reconnaissance |
| Maltego Graph | Visual OSINT and relationship mapping |
| theHarvester | OSINT and reconnaissance |
| Zenmap | Network discovery and scanning |
| Nmap | Network scanning engine |


Evidence

The repository contains supporting documentation and evidence for the Week 2 practical activities.

Module Evidence

- [PM1 — Multiple Kali Tools](./PM1-Multiple-Kali-Tools/)
- [PM2 — GHDB](./PM2-GHDB/)
- [PM3 — Maltego](./PM3-Maltego/)
- [PM4 — theHarvester](./PM4-theHarvester/)
- [PM5 — Zenmap](./PM5-Zenmap/)

Final Report

The detailed Week 2 report is available in:

[Final Report](./Final-Report/)


Key Learning Areas

The Week 2 activities provided practical exposure to:

- Passive reconnaissance
- Domain and DNS enumeration
- Web technology identification
- WAF detection
- Search-engine reconnaissance
- OSINT techniques
- Visual reconnaissance with Maltego
- Email and host enumeration
- Network discovery
- IP and MAC address identification
- Network topology visualization
- Evidence collection and documentation


Scope & Responsible Use

The activities documented in this repository were performed for educational and authorized cybersecurity training purposes.

Reconnaissance and scanning activities should only be performed against systems, networks, and information for which appropriate authorization has been provided.


Internship

**Networkwalks Cybersecurity Internship — Batch B083**

**Mentor/Instructor:** Waqas Karim CCIE


Author

**Dan Ngechu**

Cybersecurity Intern  
Networkwalks Academy
