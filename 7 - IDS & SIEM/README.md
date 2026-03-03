# Module 7 - IDS & SIEM

## Objective
Deploy and configure intrusion detection and SIEM tools in a home lab environment. Ingest real Active Directory logs into Splunk, write detection rules, and build dashboards for monitoring security events.

> **Home Lab Focus:** My SIEM module is built around my actual Active Directory lab. I ingest real Windows event logs from my domain controller into Splunk Free tier and write detection logic for real AD-based threats (failed logins, account lockouts, privilege escalation).

## Skills Demonstrated
- Intrusion Detection System (IDS) Configuration
- SIEM Log Ingestion & Parsing
- Splunk Search Processing Language (SPL)
- Splunk Dashboard & Alert Creation
- Suricata Rule Writing
- Windows Event Log Analysis (Event IDs 4624, 4625, 4740, etc.)
- Chronicle (Google Security Operations)
- Threat Detection Logic

## Tools Used
- Splunk Free (SIEM)
- Suricata (IDS)
- Chronicle
- Windows Server 2025 (log source)
- Linux CLI

## Lab Architecture
- Log Source: Windows Server 2025 (Active Directory Domain Controller)
- SIEM: Splunk Free tier
- Forwarding: Splunk Universal Forwarder on Windows Server
- Dashboards: Failed logins, account lockouts, privilege escalation patterns

## Projects
- 7.1 - Splunk: Ingest Active Directory Logs *(in progress)*
- 7.2 - Splunk: Build Security Dashboard *(in progress)*
- 7.3 - Splunk: Write Correlation Alerts *(in progress)*
- 7.4 - Suricata: Write Custom IDS Rules *(in progress)*
- 7.5 - Chronicle: Investigate Security Event *(in progress)*

## Status
> Lab configured. Splunk ingestion in progress. Write-up coming soon.
