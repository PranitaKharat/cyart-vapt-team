# Vulnerability Assessment and Penetration Testing Report

## Executive Summary

A vulnerability assessment and penetration testing activity was conducted on the target system to identify potential security weaknesses. The testing revealed several vulnerabilities including SQL Injection and insecure services running on open ports.

## Scope

Target System: Metasploitable2  
Testing Machine: Kali Linux

## Tools Used

- Nmap
- Metasploit
- Burp Suite
- SQLMap
- Wireshark

## Technical Findings

| Finding ID | Vulnerability | CVSS Score | Remediation |
|------------|--------------|------------|-------------|
| F001 | SQL Injection | 9.1 | Implement input validation |
| F002 | Open FTP Service | 7.5 | Disable unnecessary services |
| F003 | Weak Authentication | 6.8 | Enforce strong passwords |

## Recommendations

- Implement proper input validation
- Disable unused services
- Update vulnerable software
- Apply regular security patches

## Conclusion

The assessment successfully identified multiple vulnerabilities in the target environment. Proper remediation steps should be implemented to improve the overall security posture.
