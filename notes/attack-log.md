# Attack Log

## 1. Baseline Traffic
- Source: Kali container
- Target: DVWA web server
- Actions:
  - HTTP request using curl
  - ICMP ping
  - login page request
- PCAP file: baseline.pcap
- Outcome: Baseline HTTP and ICMP traffic captured successfully.

## 2. Nmap SYN Scan
- Source: Kali container
- Target: DVWA web server
- Command: `nmap -sS dvwa`
- PCAP file: nmap-scan.pcap
- Outcome: Host reachable and port 80/tcp identified as open.

## 3. Brute Force Login Simulation
- Source: Kali container
- Target: DVWA brute-force endpoint
- Method: repeated HTTP POST requests
- PCAP file: bruteforce.pcap
- Outcome: Repeated login traffic generated for analysis.

## 4. SQL Injection
- Status: planned or partially attempted
- Note: browser-side capture workflow required for reliable host-level capture.

## 5. XSS
- Status: planned or partially attempted
- Note: browser-side capture workflow required for reliable host-level capture.