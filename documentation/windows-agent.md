# Windows Agent Configuration

## Overview

The Windows endpoint serves as the primary monitored system within the lab.

The Wazuh agent collects security-relevant telemetry from the endpoint and forwards events to the Wazuh monitoring environment.

## Endpoint

- Operating System: Windows 11
- Hostname: Nathaniel
- Wazuh Agent: Installed
- Status: Active

## Agent Configuration

The Wazuh agent was installed on the Windows endpoint and configured to communicate with the Wazuh monitoring environment.

The agent provides visibility into Windows security and system activity.

## Data Sources

The monitoring environment uses several Windows data sources, including:

- Windows Security Event Logs
- Windows System Events
- Windows Application Events
- Sysmon telemetry
- PowerShell activity

## Monitored Activity

The endpoint was monitored for:

- Authentication attempts
- Account changes
- Process execution
- PowerShell activity
- File activity
- Network activity

## Verification

The Wazuh dashboard was used to verify that the Windows endpoint was successfully connected and actively reporting events.

![Windows Agent](../screenshots/windows-agent.png)
