PM4 — Footprinting & Reconnaissance with theHarvester

Module Overview

This module focused on passive footprinting and reconnaissance using **theHarvester** in Kali Linux.

The objective was to collect publicly available information associated with the target domain without directly attacking the target.

Internship Information

- **Program:** Networkwalks Cybersecurity Internship
- **Batch:** B083
- **Participant:** Dan Ngechu
- **Module:** Week 2 — PM4
- **Tool:** theHarvester
- **Operating System:** Kali Linux

Objectives

The module consisted of two reconnaissance tasks:

1. Search for email addresses and subdomains associated with `microsoft.com` using the Baidu source with a search limit of 1000.
2. Search for email addresses and subdomains associated with `microsoft.com` using all available sources with a search limit of 50.

Task 1 — Baidu Reconnaissance

Command

`theHarvester -d microsoft.com -l 1000 -b baidu`

Target

`microsoft.com`

Source

`Baidu`

Search Limit

`1000`

Result

The tool completed the search against the Baidu source.

Observed results:

- No IP addresses found
- No email addresses found
- No people found
- No hosts found

Saved Output

The command output was saved locally as:

`pm4-task1-baidu.txt`

The output was also verified using:

`cat pm4-task1-baidu.txt`

Task 2 — All Sources Reconnaissance

Command

`theHarvester -d microsoft.com -l 50 -b all`

Target

`microsoft.com`

Sources

`all`

Search Limit

`50`

Result

The scan produced extensive reconnaissance output containing information from multiple public sources.

The results included numerous Microsoft-related subdomains and hostnames.

Examples observed during the scan included:

- `z29.dxt-c.fabric.microsoft.com`
- `z31.daily-dfs.fabric.microsoft.com`
- `z3d.blob.fabric-df.microsoft.com`
- `z3e.dxt-datawarehouse.fabric.microsoft.com`
- `z46.dxt-c.fabric.microsoft.com`
- `z50.sql.cosmos.fabric.microsoft.com`
- `z62.dxt-onelake.fabric.microsoft.com`
- `zai-prod-mwh-proc.ait.microsoft.com`
- `zebra-ai-api-prd.ait.microsoft.com`
- `zebra-ai-web-prd.ait.microsoft.com`
- `zeus.buddy.microsoft.com`
- `zf9.blob.fabric.microsoft.com`

The scan also reported that several data sources required API keys or additional configuration.

Saved Output

The complete output was captured using:

`theHarvester -d microsoft.com -l 50 -b all 2>&1 | tee pm4-task2-all.txt`

The resulting file contained approximately **10,299 lines** of output.

Evidence

Evidence collected for this module includes:

- Task 1 theHarvester output
- Task 2 complete theHarvester output
- `pm4-task1-baidu.txt`
- `pm4-task2-all.txt`
- Terminal screenshots where applicable

The complete raw Task 2 output is retained separately as working evidence rather than being included directly in this public repository.

Scope

The reconnaissance activities were performed as part of the assigned Networkwalks Week 2 educational module.

TheHarvester was used for passive information gathering from publicly available sources. No exploitation or intrusive activity was performed as part of these tasks.

Responsible Use

Reconnaissance tools should only be used against domains and systems where the user has appropriate authorization or where the activity is explicitly permitted for educational purposes.

Information discovered during reconnaissance should be handled responsibly and should not be used to access, disrupt, or compromise systems.

Module Status

**Completed**

Author

**Dan Ngechu**

Networkwalks Cybersecurity Internship — Batch B083
