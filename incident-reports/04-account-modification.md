Endpoint: WIN-11-LAB
Date: June 2, 2026
User Created: TestUser
Created By: Nathaniel
Windows Event ID: 4720
Privilege Change: Added to Administrators group
Windows Event ID: 4732
Severity: High
MITRE ATT&CK: T1136.001 - Create Account: Local Account

FINDINGS: A new local Windows account named TestUser was created during controlled testing. The account was subsequently added to the local Administrators group to test detection of account and privilege changes.


Account:
TestUser

Created by:
Nathaniel

Account type:
Local

Privilege:
Local Administrator

Events:
4720 - User account created
4732 - Member added to security-enabled local group
