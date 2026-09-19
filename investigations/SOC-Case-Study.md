# SOC Investigation Case Study

## Incident Overview

A Windows security monitoring investigation was performed using Wazuh SIEM.

The investigation focused on authentication activity, failed logon events, successful logons, and process creation events observed from a Windows endpoint.

## Environment

- SIEM: Wazuh
- Endpoint: Windows
- Virtualization: VirtualBox
- Analysis Tools: Wazuh Threat Hunting, Windows Event Logs, PowerShell

## Detection

The investigation started from security events collected by Wazuh from the Windows endpoint.

Relevant events included:

- Event ID 4625 – Failed Logon
- Event ID 4624 – Successful Logon
- Event ID 4688 – Process Creation

## Investigation Process

Alert
↓
Validate Event
↓
Collect Evidence
↓
Correlate Related Events
↓
Build Timeline
↓
Investigate Activity
↓
Document Findings

## Event Analysis

### Event ID 4625

Failed authentication activity was reviewed using:

- Username
- Timestamp
- Logon Type
- Failure Reason
- Source IP, when available

The event was treated as an investigation lead rather than automatically classified as an attack.

### Event ID 4624

Successful authentication activity was reviewed using:

- Username
- Timestamp
- Logon Type
- Authentication details
- Related events

A successful logon alone was not treated as malicious.

### Event ID 4688

Process creation activity was reviewed using:

- New Process Name
- Parent Process
- Process ID
- Command Line, when available
- User context
- Related activity

Process creation was evaluated using process context and related events.

## Investigation Findings

The investigated events provided visibility into authentication and process activity on the Windows endpoint.

Event correlation and surrounding context were considered before determining whether activity was suspicious.

## Skills Demonstrated

- SIEM Monitoring
- Log Analysis
- Alert Triage
- Threat Hunting
- IOC Investigation
- Event Correlation
- Incident Investigation
- MITRE ATT&CK Analysis

## Conclusion

This case study demonstrates a practical SOC investigation workflow using Wazuh to monitor and investigate Windows security events.
