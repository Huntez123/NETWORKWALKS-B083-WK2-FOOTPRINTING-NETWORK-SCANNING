Week 2 Final Report — Footprinting & Network Scanning

Project Overview

This repository documents the Week 2 cybersecurity internship activities completed under the Networkwalks Academy program.

The project covered multiple footprinting, reconnaissance, and network-scanning techniques using Kali Linux and Windows-based security tools.

Internship Information

- **Program:** Networkwalks Cybersecurity Internship
- **Batch:** B083
- **Participant:** Dan Ngechu
- **Week:** 2
- **Date:** 18 September 2026
- **Mentor:** Waqas Karim CCIE

Modules Completed

All five Week 2 project modules were completed:

| Module | Topic | Target |
|---|---|---|
| PM1 | Footprinting & Reconnaissance with Multiple Kali Tools | `networkwalks.com` |
| PM2 | Footprinting & Reconnaissance with GHDB | Google Hacking Database |
| PM3 | Footprinting with Maltego | `networkwalks.com` |
| PM4 | Footprinting & Reconnaissance with theHarvester | `microsoft.com` |
| PM5 | Network Scanning with Zenmap | Local LAN `192.168.1.0/24` |

PM1 — Multiple Kali Tools

The first module focused on reconnaissance using multiple Kali Linux tools.

Tools used:

- `whois`
- `WhatWeb`
- `nslookup`
- `curl`
- `wafw00f`
- `dnsrecon`

The activities collected publicly available information about the target domain and demonstrated different reconnaissance techniques.

PM2 — Google Hacking Database

The second module focused on Google Hacking Database techniques.

The activities involved using search-engine queries to identify publicly indexed resources, including:

- Security-camera-related resources
- Publicly accessible mathematics PDF directories

Seven documented findings were retained for each task based on the results obtained during the exercise.

Specific third-party camera URLs and authentication information are intentionally not reproduced in this public repository.

PM3 — Maltego

The third module introduced Maltego for graphical reconnaissance and relationship mapping.

The target domain was:

`networkwalks.com`

The following Maltego transforms were tested:

- `[Utilities] To Emails @domain [Search Engine]`
- `[Utilities] To E-Mail Addresses [within Properties]`

Both transforms completed successfully during the exercise, but no Email Address entity was returned in the resulting graph.

The observed graph and Maltego activity were documented as project evidence.

PM4 — theHarvester

The fourth module used theHarvester for passive reconnaissance against:

`microsoft.com`

Two searches were performed.

Task 1

`theHarvester -d microsoft.com -l 1000 -b baidu`

The Baidu search completed with no IP addresses, email addresses, people, or hosts returned.

Task 2

`theHarvester -d microsoft.com -l 50 -b all`

The all-source search produced extensive reconnaissance output containing numerous Microsoft-related hostnames and subdomains.

The complete raw output was retained separately as working evidence.

PM5 — Zenmap

The fifth module focused on network scanning using Zenmap.

The local LAN was identified as:

`192.168.1.0/24`

A Ping Scan was performed using:

`nmap -sn 192.168.1.0/24`

Four live hosts were identified:

- `192.168.1.1`
- `192.168.1.3`
- `192.168.1.7`
- `192.168.1.8`

The corresponding IP and MAC address information was documented, and a network topology was generated and exported as a PDF.

Tools Used

The Week 2 activities used the following tools and technologies:

- Kali Linux
- VirtualBox
- WHOIS
- WhatWeb
- nslookup
- curl
- wafw00f
- dnsrecon
- Google Hacking Database
- Maltego
- theHarvester
- Zenmap
- Nmap
- Windows Command Prompt

Repository Structure

The repository is organized by project module:

- `PM1-Multiple-Kali-Tools/` — Multiple Kali reconnaissance tools
- `PM2-GHDB/` — Google Hacking Database reconnaissance
- `PM3-Maltego/` — Maltego reconnaissance
- `PM4-theHarvester/` — theHarvester reconnaissance
- `PM5-Zenmap/` — Zenmap network scanning
- `Final-Report/` — Week 2 final report documentation

Evidence

Project evidence includes:

- Terminal outputs
- Reconnaissance results
- Maltego graph evidence
- Zenmap scan results
- IP and MAC address records
- Network topology PDF
- Working documentation
- Final project report

Raw evidence containing unnecessary third-party information is retained separately and is not published in this public repository.

Scope and Responsible Use

The activities documented in this repository were conducted as part of an authorized cybersecurity training program.

Reconnaissance and network-scanning techniques should only be performed against systems, domains, or networks where appropriate authorization has been granted.

Information discovered during security testing should be handled responsibly and should not be used to access, disrupt, or compromise systems without authorization.

Final Report

The complete Week 2 final report is maintained separately from the individual module documentation.

The report covers:

- Introduction
- Scope and authorization
- Tools used
- PM1 reconnaissance
- PM2 GHDB reconnaissance
- PM3 Maltego reconnaissance
- PM4 theHarvester reconnaissance
- PM5 Zenmap network scanning
- Findings and observations
- Risk and impact considerations
- Recommendations
- Conclusion
- Evidence collected

Project Status

**Week 2 — Completed**

All five assigned project modules were completed and documented.

Author

**Dan Ngechu**

Networkwalks Cybersecurity Internship — Batch B083
