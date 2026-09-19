# Wazuh Security Event Investigations

This section documents security event investigations performed in the Wazuh SOC home lab.

## Investigations

### Event ID 4625 – Failed Logon

- Event ID: 4625
- Description: Failed authentication attempt
- Investigation focus:
  - Username
  - Timestamp
  - Logon Type
  - Failure Reason
  - Source IP, when available
  - Related authentication events

![4625 Failed Logon](../screenshots/event-4625-failed-logon.png)

---

### Event ID 4624 – Successful Logon

- Event ID: 4624
- Description: Successful authentication
- Investigation focus:
  - Username
  - Timestamp
  - Logon Type
  - Authentication details
  - Related events

![4624 Successful Logon](../screenshots/event-4624-successful-logon.png)

---

### Event ID 4688 – Process Creation

- Event ID: 4688
- Description: New process creation
- Investigation focus:
  - New Process Name
  - Parent Process
  - Process ID
  - Command Line, when available
  - User context
  - Related network activity

![4688 Process Creation](../screenshots/event-4688-process-creation.png)

## Investigation Approach

Alert → Validate → Collect Evidence → Correlate → Build Timeline → Investigate → Document Findings
