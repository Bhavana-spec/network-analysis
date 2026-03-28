# Architecture Limitations and Design Decisions

This lab was built on Docker Desktop for macOS using DVWA, Kali Linux, Wireshark, and Suricata.

During testing, Suricata running as a separate sensor container did not reliably observe all East-West traffic between the Kali and DVWA containers through passive live sniffing alone.

Because of this limitation, the project evolved toward a hybrid workflow:
- live traffic generation and capture
- packet inspection using Wireshark
- IDS validation using Suricata logs
- offline PCAP-based signature analysis

This design decision improved reproducibility and made the lab more realistic for a desktop container environment.