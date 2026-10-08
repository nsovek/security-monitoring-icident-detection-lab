Source:
192.168.56.103

Target:
192.168.56.10

Date:
June 11, 2026

Tool:
Nmap

Scan:
TCP SYN scan

MITRE ATT&CK:
T1046 - Network Service Scanning

22/tcp    open    ssh
80/tcp    open    http
135/tcp   open    msrpc
445/tcp   open    microsoft-ds
3389/tcp  open    ms-wbt-server


FINDINGS: A controlled Nmap scan was performed from the Windows endpoint against the lab network. The scan identified several accessible services and was used to evaluate visibility into network reconnaissance activity.
