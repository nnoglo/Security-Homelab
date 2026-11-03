# Wazuh Home Lab: SIEM and Threat Detection
## Architecture
| Machine | Role | IP |
|---|---|---|
| Wazuh Server (Ubuntu Server 22.04 VM) | Analyst: SIEM (manager, indexer, dashboard) | 10.0.2.3 |
| Ubuntu Server 22.04 VM | Monitored endpoint (Linux agent) | 10.0.2.4 |
| Windows 11 host | Monitored endpoint (Windows agent), reaches the server via port forwarding | 127.0.0.1 (forwarded) |
| Kali Linux VM | Attacker machine (planned for this project) | not yet on this network |

## Tools Used
* Wazuh 4.14 (SIEM): Server, indexer, and dashboard on one VM.
* Wazuh agents: Ubuntu Server VM and Windows 11 host.
* Ubuntu Server 22.04 LTS (x86_64): Wazuh Server and Linux Agent.
* VirtualBox on Windows: Hypervisor, with a NAT Network connecting the VMS.
* OpenSSH, VBoxManage, PowerShell: Remote access, port forwarding, and agent deployment.

## Log Sources Monitored

## Attacks Simulated

## Incident Reports

## Skills Demonstrated
* Deploying and configuring a Wazuh SIEM (server, indexer, dashboard)
* Enrolling and managing Wazuh agents on Linux and Windows endpoints
* Virtual network design: VirtualBox NAT Network, port forwarding with VBoxManage
* Linux administration (Ubuntu Server): SSH, systemd services, partition and filesystem resizing, swap configuration, config file editing
* Troubleshooting with logs and diagnostics (ossec.log, du/df, ip, ping)
* Resource and capacity planning on constrained hardware (8 GB RAM)
* Technical documentation of builds, problems, and fixes

###
## In Progress
- SSH brute-force detection (Kali Hydra against the Ubuntu agent)
- Port scan detection (Nmap)
- Windows event log analysis (failed logons, account changes)
- Custom Wazuh detection rule
- Mapping alerts to MITRE ATT&CK techniques
## Repository Structure
