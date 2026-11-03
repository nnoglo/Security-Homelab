# Security Homelab

A virtualized home lab for learning defensive security. I build and monitor
systems with a Wazuh SIEM, document what breaks, and write up how I fixed it.
The goal is hands-on experience with log monitoring and detection, aimed at
blue-team and SOC analyst work.

## Lab Environment

- Host: Windows laptop with 8 GB RAM, running VirtualBox
- VMs: Ubuntu Server 22.04 LTS (Wazuh server and Linux agent), Kali Linux
- Network: VirtualBox NAT Network, with services published to the host
  only on 127.0.0.1
- Constraint: 8 GB RAM, so I run one or two VMs at a time. That shaped
  several design choices, which are covered in the project write-ups.

## Projects

| Project | What it covers | Status |
|---|---|---|
| [Wazuh SIEM](https://github.com/nnoglo/Security-Homelab/tree/main/Wazuh) | SIEM with Linux and Windows agents, attack simulation, detection | In progress |
| Pi-hole, Tailscale, Docker | Network services and remote access | Planned |
