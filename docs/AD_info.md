## Info about infra

| VM Name                   | OS             | IP         | Role          |
| ------------------------- | -------------- | ---------- | ------------- |
| Arachne-DC                | Windows Server | 10.0.0.5   | AD / DNS      |
| Arachne-bastion           | Ubuntu Server  | 10.0.0.10  | SSH + Ansible |
| Arachne-docker            | Ubuntu Server  | 10.0.0.20  | Docker        |
| Arachne-wazuh             | Ubuntu Server  | 10.0.0.30  | SIEM          |
| Arachne-Onion-work        | Security Onion | 10.0.0.103 | NIDS          |
| Arachne-win11-client      | Win11          | 10.0.0.100 | User          |
| Arachne-win11-compromised | Win11          | 10.0.0.102 | Victim        |
| Arachne-Ubuntu-client     | Ubuntu Desktop | 10.0.0.101 | User          |
