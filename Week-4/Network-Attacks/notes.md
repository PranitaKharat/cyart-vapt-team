# Network Protocol Attacks Lab

## Objective
To observe network-level attack techniques such as credential capture and traffic interception in a controlled lab environment.

## Target Details
- **Attacker IP:** 192.168.56.103
- **Target IP:** 192.168.56.102

## Tools Used
- Responder
- Ettercap
- Wireshark
- Kali Linux

## Steps Performed
1. Verified attacker network interface configuration.
2. Used Responder to listen for and capture authentication attempts on the local network.
3. Observed captured NTLM hash information from network activity.
4. Used ARP spoofing concepts to position the attacker between communicating systems.
5. Inspected traffic flow and documented the security risk.

## Screenshot Reference
- `ifconfig.png` – Attacker interface/network information
- `responder_hash.png` – Hash capture evidence
- `arp_spoof.png` – ARP spoofing / MitM evidence

## Log Entry
| Attack ID | Technique  | Target IP      | Status  | Outcome            |
|-----------|------------|----------------|---------|--------------------|
| 015       | SMB Relay / Hash Capture | 192.168.56.102 | Success | NTLM Hash Captured |

## MitM Summary 
Man-in-the-middle style interception allows an attacker to observe or relay communication between systems on the same network. Capturing authentication material and spoofing network relationships demonstrate the impact of insecure local protocols. Network segmentation, strong authentication, and encrypted communication are essential to reduce these risks.

## Checklist
- [x] Verified interface settings
- [x] Captured hash/network evidence
- [x] Observed ARP spoofing activity
- [x] Documented network attack screenshots

## Conclusion
This lab showed how weak trust relationships and broadcast-based authentication can be abused in local networks. Defensive controls such as SMB signing, segmentation, and encrypted protocols significantly reduce exposure.
