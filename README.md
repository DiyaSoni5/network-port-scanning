# network-port-scanning
# Network Port Scanning & DNS Traffic Analysis

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

 ### 📊 Key Observations
- **Captured DNS Traffic**: Request and response for several domains
- **Filter Used**: `udp.port == 53`
- **Source IP**: 192.168.44.128 (Host)
- **Destination IP**: 192.168.44.2 (DNS server)
- **Query Highlight**: `www.google.com`

### 📷 Screenshot
Below is a Wireshark screenshot showing a DNS query made to `www.google.com`:

![DNS Screenshot](wireshark_dns_screenshot.png)


## Security Recommendations
- Restrict access to the DNS service to trusted IP addresses.
- Regularly update the DNS software to patch vulnerabilities.
- Monitor DNS traffic for unusual patterns.

## Conclusion
This task provided insights into network exposure and highlighted the importance of securing open ports.

### 🛠 Tools Used
- Kali Linux
- Wireshark
- GitHub for hosting files and report

