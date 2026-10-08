# Security Monitoring & Incident Detection Lab

A hands-on cybersecurity lab focused on security monitoring, endpoint detection, log analysis, and incident investigation using Wazuh.

## Project Overview

This project demonstrates the setup and operation of a security monitoring environment using Wazuh to collect, analyze, and investigate security events from a Windows endpoint.

The lab was designed to simulate common security monitoring scenarios and provide practical experience with endpoint telemetry, security alerts, event investigation, and incident documentation.

## Objectives

The primary objectives of this lab are to:

- Monitor Windows security events
- Detect authentication activity
- Analyze PowerShell execution
- Monitor process execution
- Detect account and user modifications
- Monitor file activity
- Analyze network reconnaissance
- Investigate security alerts
- Map activity to MITRE ATT&CK techniques
- Document security incidents and findings

## Technologies

- Wazuh
- Windows 11
- Sysmon
- PowerShell
- Nmap
- Windows Event Logs
- MITRE ATT&CK
- Virtualization

## Lab Architecture

The environment consists of a Windows endpoint monitored by Wazuh. Windows Event Logs and Sysmon telemetry are collected and analyzed by the Wazuh platform.

![Lab Architecture](architecture/lab-architecture.png)

## Security Monitoring

### Wazuh Dashboard

![Wazuh Dashboard](screenshots/dashboard-overview.png)

### Windows Endpoint

![Windows Agent](screenshots/windows-agent.png)

## Detection Scenarios

| Scenario | Technology | Detection |
|---|---|---|
| Authentication | Windows Event Logs | Failed and successful authentication |
| PowerShell Activity | Sysmon / Windows Logs | PowerShell execution |
| Process Execution | Sysmon | Process creation |
| Account Modification | Windows Security Logs | User creation and privilege changes |
| File Modification | Wazuh FIM | File creation and modification |
| Network Reconnaissance | Nmap | Network scanning activity |

## Incident Investigations

The incident reports in this repository document the investigation process, evidence, affected systems, security findings, and recommended remediation.

- [Authentication Failures](incident-reports/01-authentication-failures.md)
- [PowerShell Activity](incident-reports/02-powershell-activity.md)
- [Process Execution](incident-reports/03-process-execution.md)
- [Account Modification](incident-reports/04-account-modification.md)
- [File Modification](incident-reports/05-file-modification.md)
- [Network Reconnaissance](incident-reports/06-network-reconnaissance.md)

## Documentation

- [Lab Setup](documentation/setup.md)
- [Windows Agent Configuration](documentation/windows-agent.md)
- [Sysmon Configuration](documentation/sysmon-configuration.md)
- [Wazuh Configuration](documentation/wazuh-configuration.md)

## Key Skills Demonstrated

- Security monitoring
- SIEM administration
- Log analysis
- Endpoint monitoring
- Windows security
- Incident detection
- Network reconnaissance
- MITRE ATT&CK mapping
- Security event investigation
- Incident documentation
