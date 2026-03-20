# Privilege Escalation and Persistence Lab

## Objective
To identify privilege escalation opportunities using enumeration tools and validate elevated access on the target machine.

## Target Details
- **Attacker IP:** 192.168.56.103
- **Target IP:** 192.168.56.102

## Tools Used
- LinPEAS
- Kali Linux
- Meterpreter / Shell

## Steps Performed
1. Accessed the target machine after exploitation.
2. Performed local enumeration to identify misconfigurations and privilege escalation vectors.
3. Used LinPEAS to collect system privilege information.
4. Reviewed SUID binaries, permissions, and configuration weaknesses.
5. Obtained elevated/root-level access on the target.
6. Verified the result using shell commands.

## Screenshot Reference
- `linpeas_scan.png` – LinPEAS enumeration output
- `root_access.png` – Proof of elevated access
- `post_exploitation.png` – Additional shell/session evidence

## Log Entry
| Task ID | Technique     | Target IP      | Status  | Outcome    |
|---------|---------------|----------------|---------|------------|
| 010     | SUID Exploit  | 192.168.56.102 | Success | Root Shell |

## Persistence Summary 
Persistence can be maintained by creating a scheduled task or cron job that executes a reverse shell or command at regular intervals. This ensures that access can be regained after reboot or session loss. Such techniques highlight the need for monitoring scheduled tasks and restricting unauthorized system modifications.

## Checklist
- [x] Ran LinPEAS for local enumeration
- [x] Reviewed privilege escalation vectors
- [x] Confirmed elevated/root access
- [x] Documented post-exploitation evidence

## Conclusion
This exercise demonstrated the importance of post-exploitation enumeration and the risks created by weak permissions or misconfigured privileged binaries. Proper hardening, auditing, and least-privilege controls are necessary to prevent escalation.
