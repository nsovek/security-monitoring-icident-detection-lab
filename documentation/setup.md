# Lab Setup

## Overview

This document describes the process used to build the security monitoring and incident detection laboratory.

The environment consists of a Wazuh monitoring platform and a Windows endpoint used to generate controlled security events for detection and investigation.

## Environment

### Monitoring Platform

- Wazuh
- Wazuh Dashboard
- Wazuh Manager
- Wazuh Indexer

### Endpoint

- Windows 11
- Wazuh Agent
- Sysmon
- Windows Event Logs
- PowerShell

### Security Tools

- Nmap
- MITRE ATT&CK

## Setup Process

### 1. Wazuh Deployment

Wazuh was deployed and configured as the central security monitoring platform.

The Wazuh environment provides:

- Security event collection
- Alert generation
- Event analysis
- Security dashboards
- Threat investigation
- MITRE ATT&CK mapping

### 2. Windows Endpoint

A Windows 11 endpoint was configured as the monitored system.

The endpoint was connected to Wazuh using the Wazuh agent.

### 3. Windows Event Logging

Windows security and system events were configured for collection and analysis.

The monitored events include authentication activity, account changes, process activity, and other security-relevant events.

### 4. Sysmon

Sysmon was configured on the Windows endpoint to provide additional telemetry related to:

- Process creation
- Process relationships
- Network connections
- File activity
- PowerShell activity

### 5. Controlled Security Testing

Controlled security events were generated on the endpoint to test the monitoring environment.

Testing included:

- Authentication failures
- PowerShell activity
- Process execution
- Account modifications
- File activity
- Network reconnaissance

### 6. Alert Investigation

Generated events were reviewed in the Wazuh dashboard.

Investigations focused on:

- Timestamp
- Affected endpoint
- Username
- Process
- Event information
- Alert severity
- MITRE ATT&CK mapping

## Validation

The environment was validated by generating controlled events and confirming that relevant telemetry and alerts appeared within Wazuh.

Screenshots and investigation results are documented throughout this repository.
