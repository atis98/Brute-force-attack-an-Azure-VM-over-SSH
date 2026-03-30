# This document shows the steps of a brute-force attack in a TEST environment against an Azure Virtual Machine using Netcrack and rockyou.txt
## Adversary device: my own PC running Windows 10 Pro.
## Attacked device: an Azure Virtual Machine running Linux, in my own Azure subscription.
## Attack method: brute-force the administrator account password using Netcrack and rockyou.txt
## Exploited vulnerabilities: left-open SSH port and weak password
## MITRE ATT&CK tactic used: TA0006: Credentials Access
## Attack steps:
- I created an Azure VM with Linux. In the network settings, I left the SSH port 22 open for inbound traffic.
- I used the nmap command on my PC to check the open ports of the VM (using its public IP address)
