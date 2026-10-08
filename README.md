# Security Monitoring & Incident Detection Lab

A hands-on cybersecurity lab focused on security monitoring, endpoint detection, log analysis, and incident investigation using Wazuh.

## Project Overview

This project demonstrates the setup and operation of a security monitoring environment using Wazuh to collect, analyze, and investigate security events from a Windows endpoint.

The lab focuses on detecting and investigating:

- Authentication failures and successful logins
- PowerShell activity
- Process execution
- User and account modifications
- File modifications
- Network activity and reconnaissance
- Security alerts and severity levels
- MITRE ATT&CK techniques
- Event timestamps and affected systems

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

The lab consists of a Wazuh monitoring environment connected to a Windows endpoint. Security events generated on the endpoint are collected and analyzed by Wazuh.

![Lab Architecture](architecture/lab-architecture.png)

## Security Monitoring

### Wazuh Dashboard

![Wazuh Dashboard](screenshots/dashboard-overview.png)

### Windows Endpoint

![Windows Agent](screenshots/windows-agent.png)

## Detection Scenarios

| Scenario | Technology | Detection |
|---|---|---|
| Authentication | Windows Event Logs | Failed and successful login attempts |
| PowerShell Activity | Sysmon / Windows Logs | PowerShell execution |
| Process Execution | Sysmon | Process creation |
| Account Modification | Windows Security Logs | User creation and privilege changes |
| File Modification | Wazuh FIM | File creation and modification |
| Network Reconnaissance | Nmap | Network scanning activity |

## Incident Investigations

Detailed incident reports will document the investigation process, findings, affected systems, and recommended remediation.

- Authentication Failures
- PowerShell Activity
- Process Execution
- Account Modification
- File Modification
- Network Reconnaissance

## Key Skills Demonstrated

- Security monitoring
- SIEM administration
- Log analysis
- Incident detection
- Windows security
- Endpoint monitoring
- Network reconnaissance
- MITRE ATT&CK mapping
- Incident documentation
