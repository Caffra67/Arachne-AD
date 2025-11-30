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
| Name               | Role                                | Operating System           |
| ------------------ | ----------------------------------- | -------------------------- |
| **DC**             | Domain Controller                   | Windows Server 2025        |
| **Win11-User**     | Domain user workstation             | Windows 11 Enterprise      |
| **Win11-User-Vul** | Testing / vulnerable workstation    | Windows 11 Enterprise      |
| **Ubuntu-Desktop** | Linux workstation                   | Ubuntu 22.04 Desktop       |
| **Ubuntu-Server**  | Internal service / intranet hosting | Ubuntu Server 22.04        |
| **Security-Onion** | IDS / SIEM                          | Security Onion             |
| **Attacker**       | External attacker machine           | Arch Linux                 |

## Architecture
Network Topology

TODO

## Attack Scenarios (MITRE ATT&CK)
Directory: scenarios/

**Included Scenarios**
- TODO

## Detection & Monitoring
Directory: detection/

TODO

## Provisioning & Automation
Directory: provisioning/

## Documentation
Directory: docs/
