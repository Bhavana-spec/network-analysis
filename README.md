# SOC-Style Network Traffic Analysis Lab

## Overview
This project is a hands-on network traffic analysis and IDS validation lab built using Docker, Kali Linux, DVWA, Wireshark, and Suricata.

The lab was designed to simulate attacker-target traffic, capture packet-level evidence, inspect suspicious patterns, and validate IDS behavior in a controlled environment.

## Objectives
- Build a reproducible attacker-target lab using containers
- Capture and inspect baseline and suspicious traffic
- Simulate reconnaissance activity using Nmap
- Analyze PCAP files in Wireshark
- Validate IDS alert generation using Suricata
- Document architecture limitations and technical findings

## Lab Components
- DVWA – vulnerable web application target
- Kali Linux – attacker container for traffic generation
- Suricata – IDS for alert generation and rule validation
- Wireshark – packet analysis
- Docker – container runtime

## Project Structure

```text
network-traffic-analysis-lab/
├── captures/
├── notes/
├── screenshots/
├── scripts/
├── suricata/
├── docker-compose.yml
├── .gitignore
└── README.md