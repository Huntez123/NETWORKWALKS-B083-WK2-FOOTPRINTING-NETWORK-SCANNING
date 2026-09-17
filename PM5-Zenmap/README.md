PM5 — Network Scanning with Zenmap

Module Overview

This module focused on network scanning and host discovery using **Zenmap**, the graphical interface for Nmap.

The objective was to identify live hosts on the local network, record their IP and MAC addresses, and generate a network topology for documentation.

Internship Information

- **Program:** Networkwalks Cybersecurity Internship
- **Batch:** B083
- **Participant:** Dan Ngechu
- **Module:** Week 2 — PM5
- **Tool:** Zenmap
- **Operating System:** Windows

Objectives

The module consisted of the following activities:

1. Install and configure Zenmap.
2. Identify the local IP address and LAN subnet.
3. Discover live hosts within the local subnet.
4. Determine the number of live hosts.
5. Record the IP addresses of discovered hosts.
6. Record the MAC addresses of discovered hosts.
7. Generate and save a network topology as a PDF.

Task 2 — Local Network Identification

The Windows network configuration was checked using:

`ipconfig`

The active Wi-Fi interface was identified with:

- **IPv4 Address:** `192.168.1.8`
- **Subnet Mask:** `255.255.255.0`
- **Default Gateway:** `192.168.1.1`

The local LAN subnet was therefore identified as:

`192.168.1.0/24`

Task 3 — Live Host Discovery

Zenmap was configured with:

- **Target:** `192.168.1.0/24`
- **Profile:** `Ping scan`

The resulting Nmap command was:

`nmap -sn 192.168.1.0/24`

The scan identified live hosts on the local network.

Task 4 — Number of Live Hosts

The scan identified **4 live hosts**.

Task 5 — Discovered IP Addresses

The following IP addresses were identified:

1. `192.168.1.1`
2. `192.168.1.3`
3. `192.168.1.7`
4. `192.168.1.8`

Task 6 — MAC Addresses

The MAC addresses associated with the discovered hosts were recorded as follows:

| IP Address | MAC Address |
|---|---|
| `192.168.1.1` | `04:7E:23:0D:FF:B0` |
| `192.168.1.3` | `6E:0B:A7:FC:08:32` |
| `192.168.1.7` | `6E:C6:87:D1:4F:2B` |
| `192.168.1.8` | `B8-8A-60-B0-6D-A0` |

Task 7 — Network Topology

Zenmap was used to generate a graphical representation of the discovered network hosts.

The topology was exported as a PDF for inclusion in the Week 2 project documentation.

The topology evidence contains the discovered local network hosts, including:

- `192.168.1.1`
- `192.168.1.3`
- `192.168.1.7`
- `192.168.1.8`

Evidence

Evidence collected for this module includes:

- Windows `ipconfig` output
- Zenmap Ping Scan results
- Discovered host information
- IP and MAC address records
- Zenmap network topology
- Exported topology PDF

Scope

The scan was performed against the participant's own local LAN:

`192.168.1.0/24`

The activity was limited to host discovery using an Nmap Ping Scan.

Responsible Use

Network scanning should only be performed against networks and systems where appropriate authorization has been obtained.

Scanning unauthorized networks or systems may violate organizational policies, laws, or acceptable-use requirements.

Module Status

**Completed**

Author

**Dan Ngechu**

Networkwalks Cybersecurity Internship — Batch B083
