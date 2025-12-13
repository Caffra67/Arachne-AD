# Arachne-AD

## Project Overview
This repository documents my personal project of building a small, realistic Active Directory environment for security research, attack simulations, and defensive analysis.
It is not a ready-made lab or a complete walkthrough instead, it contains:

- notes from the process of creating the infrastructure,
- configurations I used,
- example attack experiments I performed,
- and the defensive detections I observed.

The goal of this repository is to track my learning, improve my skills in Active Directory security, and share high-level insights with others who want to study similar topics.

## Machines Overview

| VM Name                   | OS             | IP         | Role                     |
| ------------------------- | -------------- | ---------- | ------------------------ |
| Arachne-DC                | Windows Server | 10.0.0.5   | DC                       |
| Arachne-vpn               | Ubuntu Server  | 10.0.0.254 | WireGuard VPN Gateway    |
| Arachne-bastion           | Ubuntu Server  | 10.0.0.10  | SSH + Ansible            |
| Arachne-docker            | Ubuntu Server  | 10.0.0.20  | Docker                   |
| Arachne-wazuh             | Ubuntu Server  | 10.0.0.30  | SIEM                     |
| Arachne-Onion-work        | Security Onion | 10.0.0.103 | NIDS                     |
| Arachne-win11-client      | Win11          | 10.0.0.100 | User                     |
| Arachne-win11-compromised | Win11          | 10.0.0.102 | Victim                   |
| Arachne-Ubuntu-client     | Ubuntu Desktop | 10.0.0.101 | User / Admin workstation |

## Tools
Tools used in project:
- Windows Server 2025 (AD DS, DHCP, DNS, IIS)
- WireGuard
- Wazuh
- Onion linux
- Kali linux/Black Arch tools
- OKD (Kubernetes)
- Ansible
  
## Attack Scenarios (MITRE ATT&CK)
Directory: **scenarios/**

Set of scenarios I tried/done successful

**Included Scenarios**
- TODO

## Detection & Monitoring
Directory: **detection/**

TODO

## Provisioning & Automation
Directory: **provisioning/**

Here I provide tools/commands to facilitate

## Documentation
Directory: **docs/**


## Architecture
Network Topology

TODO

