# network-port-scanning
# Network Port Scanning Task

## Objective
This repository contains the results of a network port scanning task performed using Nmap and an analysis of DNS traffic using Wireshark.

## Nmap Scan Results
- The Nmap scan was performed on the IP range `192.168.44.0/24`.
- The following hosts were found:
  - **192.168.44.1**: All ports filtered.
  - **192.168.44.2**: Port **53** open (Service: Domain).
  - **192.168.44.254**: All ports filtered.
  - **192.168.44.128**: All ports closed.

## Wireshark DNS Traffic Capture
- A capture of DNS traffic was performed to analyze the queries and responses.
- The capture file is named `dns_traffic_capture.pcap`.

## Security Recommendations
- Restrict access to the DNS service to trusted IP addresses.
- Regularly update the DNS software to patch vulnerabilities.
- Monitor DNS traffic for unusual patterns.

## Conclusion
This task provided insights into network exposure and highlighted the importance of securing open ports.
