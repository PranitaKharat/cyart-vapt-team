# Week 2 – VAPT Practical

## Objective
The objective of this lab is to understand Vulnerability Assessment and Penetration Testing (VAPT) including reconnaissance, vulnerability scanning, exploitation, and reporting.

## Tools Used
- Kali Linux
- Nmap
- Nikto
- DVWA
- SQLMap
- OpenVAS

## Step 1: Reconnaissance
Basic reconnaissance was performed to gather information about the target environment and identify available services.

## Step 2: Vulnerability Scanning
Nmap was used to scan open ports and detect running services.

Command:
nmap -sV 127.0.0.1

Nikto was used to scan the DVWA web application for vulnerabilities.

Command:
nikto -h http://localhost/dvwa

OpenVAS was configured for vulnerability scanning but the scan could not start due to feed synchronization delay.

## Step 3: Exploitation
The DVWA application was tested for SQL Injection vulnerabilities.

Payload used:
1' OR '1'='1

The injection successfully returned database records.

## Step 4: Remediation
Recommended fixes include:
- Input validation
- Prepared SQL statements
- Web application firewall
- Regular security testing

## Conclusion
The lab demonstrated how vulnerabilities can be discovered using scanning tools and exploited using penetration testing techniques.
