PM1 — Footprinting & Reconnaissance with Multiple Kali Tools

Module Overview

This module focused on footprinting and reconnaissance using multiple Kali Linux tools against the authorized Networkwalks training target.

**Target:** `networkwalks.com`

The following reconnaissance activities were performed:

- WHOIS
- WhatWeb
- nslookup
- cURL
- wafw00f
- DNSRecon

Task 1 — WHOIS

**Command:** `whois networkwalks.com`

WHOIS was used to retrieve publicly available domain registration and DNS-related information.

**Key Output:**

- Domain: `NETWORKWALKS.COM`
- Registry ID: `2452319255_DOMAIN_COM-VRSN`
- Registrar: `GoDaddy.com, LLC`
- Creation Date: `2019-11-06T22:51:46Z`
- Registry Expiry Date: `2027-11-06T22:51:46Z`
- WHOIS Server: `whois.godaddy.com`
- Name Servers: `NS6135.HOSTGATOR.COM`, `NS6136.HOSTGATOR.COM`
- DNSSEC: Unsigned

Task 2 — WhatWeb

**Command:** `whatweb networkwalks.com`

WhatWeb was used to identify technologies and web-server information associated with the target website.

**Observed Information:**

- Apache
- WordPress 7.1
- WordPress Download Manager 3.3.58
- jQuery 3.7.1
- Bootstrap 7.1
- Google Tag Manager
- HTML5
- Title: `Networkwalks Academy`
- IP Address: `192.232.216.135`
- HTTP to HTTPS redirection observed
- Contact email observed: `info@networkwalks.com`

Task 3 — nslookup

**Command:** `nslookup networkwalks.com`

nslookup was used to resolve the target domain and identify its associated IP address.

**Output:**

    Server: 8.8.8.8
    Address: 8.8.8.8#53

    Non-authoritative answer:
    Name: networkwalks.com
    Address: 192.232.216.135

Task 4 — cURL

**Command:** `curl -I https://networkwalks.com`

cURL was used to inspect the HTTP response headers returned by the target website.

**Observed Headers / Information:**

    HTTP/2 200
    server: Apache
    content-type: text/html; charset=UTF-8
    x-nginx-cache: WordPress
    x-endurance-cache-level: 0
    referrer-policy: no-referrer-when-downgrade
    link: <https://networkwalks.com/wp-json/>; rel="https://api.w.org/"

The response also exposed a WordPress REST API link and a WordPress-related cookie.

Task 5 — wafw00f

**Command:** `wafw00f https://networkwalks.com`

wafw00f was used to identify whether the target website was protected by a Web Application Firewall.

**Output:**

    [*] Checking https://networkwalks.com
    [+] The site https://networkwalks.com is behind ModSecurity (SpiderLabs) WAF.
    [~] Number of requests: 2

Task 6 — DNSRecon

**Command:** `dnsrecon -d networkwalks.com`

DNSRecon was used to enumerate publicly available DNS information associated with the target domain.

**Observed Records:**

- SOA: `ns6135.hostgator.com` — `50.87.144.87`
- NS: `ns6136.hostgator.com` — `192.232.216.131`
- NS: `ns6135.hostgator.com` — `50.87.144.87`
- MX: `mail.networkwalks.com` — `192.232.216.135`
- A: `networkwalks.com` — `192.232.216.135`
- TXT: SPF record
- TXT: Google site verification
- SRV: `_autodiscover._tcp.networkwalks.com`
- DNSSEC query returned no answer

Tools Used

| Tool | Purpose |
|---|---|
| WHOIS | Domain registration information |
| WhatWeb | Web technology identification |
| nslookup | DNS resolution |
| cURL | HTTP response/header inspection |
| wafw00f | Web Application Firewall identification |
| DNSRecon | DNS enumeration |

Evidence

Evidence was collected during each task in the form of terminal output and screenshots. Detailed raw evidence is maintained as part of the Week 2 project documentation.

Scope

**Authorized Training Target:** `networkwalks.com`

The activities in this module were performed as part of the Networkwalks Cybersecurity Internship and were limited to the scope defined by the training exercise.

Module Status

**Completed**

Networkwalks Cybersecurity Internship

**Batch:** B083  
**Participant:** Dan Ngechu  
**Module:** W2-PM1  
**Activity:** Footprinting & Reconnaissance with Multiple Kali Tools
