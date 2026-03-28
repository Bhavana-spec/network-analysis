# Incident Report

## Summary
A controlled lab environment was used to simulate suspicious traffic against a vulnerable web application. The lab included a Kali attacker container, a DVWA target container, and a Suricata IDS component.

## Activity Observed
- Baseline HTTP and ICMP traffic
- Nmap SYN scan activity
- Repeated login submission traffic
- IDS alert generation and flow logging

## Key Findings
- The DVWA host was reachable and exposed HTTP service on port 80.
- SYN scan activity was successfully generated and captured.
- Repeated login-related traffic was generated for analysis.
- Suricata successfully created logs and alerts.
- Container traffic visibility limitations affected passive monitoring design choices.

## Impact
The lab demonstrated how packet analysis and IDS validation can be used to identify normal traffic, reconnaissance behavior, and authentication-related activity in a controlled environment.

## Recommendations
- Extend the lab with authenticated DVWA testing
- Add SQL injection and XSS traffic capture
- Use offline PCAP analysis for stronger IDS validation
- Consider a VM-based segmented architecture for fuller traffic visibility