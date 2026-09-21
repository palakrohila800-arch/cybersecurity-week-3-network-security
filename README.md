# Week 3 – Advanced Cybersecurity Practical

## Project Title
Cybersecurity Week 3 – Network Security Assessment

## Objective
This project focuses on basic network security assessment and traffic investigation using Nmap and Wireshark in an authorized local environment.

## Lab Environment
- Operating System: Windows
- Target: Localhost (127.0.0.1)
- Local IPv4: 172.1.1.142
- Gateway: 172.1.1.4

## Tools Used
- Nmap
- Wireshark
- diagrams.net
- Windows Firewall

## Tasks Completed
- Task 7 – Network Discovery & Basic Nmap Scanning
- Task 8 – Advanced Nmap Security Assessment
- Task 9 – Wireshark Network Traffic Capture
- Task 10 – Nmap + Wireshark Investigation
- Task 11 – Advanced Network Traffic Investigation
- Task 12 – Vulnerability Assessment
- Task 13 – Security Hardening
- Task 14 – Final Mini Security Assessment

## Nmap Assessment
The localhost target was assessed using basic scanning, service/version detection, TCP SYN scanning, limited UDP scanning, OS detection, and vulnerability NSE scripts.

### Exposed TCP Services
- 135/tcp – msrpc
- 445/tcp – microsoft-ds
- 16992/tcp – amt-soap-http

## Wireshark Analysis
Network traffic was captured and analyzed using filters for:
- DNS
- TCP
- UDP
- ICMP
- ARP
- TCP SYN
- TCP RST

## Key Findings
The assessment identified exposed TCP services and network traffic patterns that were reviewed from a security perspective. SMB-related vulnerability checks could not complete their checks because an SMB connection could not be negotiated.

## Security Improvements
- Windows Firewall status was verified.
- An inbound firewall rule was created to block TCP port 445.
- Windows Update was completed.
- The TCP 445 localhost scan continued to show the port as open after the firewall rule, so closure was not claimed as a confirmed result.

## Before/After Results
The firewall rule was implemented and verified as enabled with a blocking action. However, the localhost Nmap scan still reported TCP 445 as open. This result was documented rather than treated as a successful port closure.

## Network Diagram
A network security assessment diagram was created using diagrams.net.

## Conclusion
This project provided practical experience with network discovery, Nmap scanning, Wireshark traffic analysis, security assessment, and basic security hardening in an authorized local environment.
