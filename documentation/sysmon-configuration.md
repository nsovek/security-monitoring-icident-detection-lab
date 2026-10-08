# Sysmon Configuration

## Overview

Sysmon was used to provide additional Windows endpoint telemetry for security monitoring and investigation.

Sysmon expands visibility beyond standard Windows Event Logs by recording detailed information about processes, network activity, and other system events.

## Purpose

The purpose of Sysmon within this lab was to improve visibility into endpoint activity and provide additional evidence during security investigations.

## Telemetry

The lab uses Sysmon telemetry to investigate activity such as:

- Process creation
- Process execution
- Parent-child process relationships
- Network connections
- PowerShell activity
- File-related activity

## Investigation Workflow

When an alert was generated, Sysmon information could be used to investigate:

1. Which process executed
2. Which user executed the process
3. The parent process
4. The process path
5. The timestamp
6. Related network activity

## Security Monitoring

Sysmon telemetry was analyzed alongside Windows Event Logs within Wazuh to provide additional context during investigations.

## Evidence

![PowerShell Detection](../screenshots/powershell-detection.png)
