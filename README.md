# Windows SOC Monitoring & Threat Detection Lab

## Overview

A hands-on SOC home lab built using Wazuh to monitor and investigate Windows security events.

This project demonstrates practical SOC activities including SIEM monitoring, log analysis, alert triage, threat hunting, IOC investigation, event correlation, and incident investigation.

## Tools Used

- Wazuh
- Windows
- PowerShell
- Wireshark
- VirtualBox

## Security Events Investigated

### Event ID 4624 – Successful Logon

Used to investigate successful authentication activity and understand:

- Username
- Timestamp
- Logon Type
- Authentication details
- Related events

### Event ID 4625 – Failed Logon

Used to investigate failed authentication attempts and analyze:

- Username
- Timestamp
- Logon Type
- Failure Reason
- Source IP, when available
- Related authentication events

### Event ID 4688 – Process Creation

Used to investigate newly created processes and analyze:

- New Process Name
- Parent Process
- Process ID
- Command Line, when available
- User context
- Related network activity

## SOC Investigation Workflow

Alert → Validate → Collect Evidence → Correlate → Build Timeline → Investigate → Document Findings

## Investigation Documentation

Detailed investigations and evidence are available in the [Investigations](./investigations/) section.

## Screenshots

Wazuh investigation screenshots are available in the [Screenshots](./screenshots/) section.

## Skills Demonstrated

- SIEM Monitoring
- Log Analysis
- Alert Triage
- Threat Hunting
- IOC Investigation
- Incident Response
- MITRE ATT&CK Analysis
- Network Investigation
- Event Correlation

## Project Status

Completed hands-on SOC home lab project focused on Windows security monitoring and investigation using Wazuh.
