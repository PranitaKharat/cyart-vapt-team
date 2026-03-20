# Capstone Project – Full VAPT Engagement

## Objective
To simulate a complete penetration testing workflow including reconnaissance, exploitation, post-exploitation, evidence collection, and reporting.

## Scope
- **Attacker IP:** 192.168.56.103
- **Target IP:** 192.168.56.102

## Tools Used
- Nmap
- Metasploit
- Burp Suite
- Kali Linux

## PTES Workflow Followed
1. Intelligence Gathering / Reconnaissance
2. Vulnerability Identification
3. Exploitation
4. Post-Exploitation
5. Reporting

## Steps Performed
1. Performed network/service discovery using Nmap.
2. Identified accessible services on the target machine.
3. Started Metasploit and selected a suitable exploit module.
4. Executed exploitation against the discovered vulnerable service.
5. Confirmed access and collected post-exploitation evidence.
6. Organized screenshots and prepared findings for reporting.

## Screenshot Reference
- `nmap_scan.png` – Nmap service discovery
- `AE1_nmap_scan.png` – Additional enumeration scan
- `exploitation.png` – Exploitation evidence
- `post_exploitation.png` – Post-exploitation/session proof

## Log Entry
| Timestamp           | Target IP      | Vulnerability | PTES Phase     |
|--------------------|----------------|---------------|----------------|
| 2026-03-20 15:00:00 | 192.168.56.102 | Service Exploitation | Exploitation |

## Remediation Recommendations
- Apply security patches to vulnerable services
- Remove or disable unnecessary services
- Enforce input validation
- Implement least privilege
- Perform regular vulnerability scanning
- Monitor logs and unauthorized access attempts

## Conclusion
The capstone activity combined multiple VAPT phases into a complete assessment workflow. It demonstrated how reconnaissance, exploitation, and evidence-based reporting work together in a professional penetration testing engagement.
