# Mobile Application Testing Lab

## Objective
To perform basic static and dynamic analysis of a mobile application using MobSF and Frida.

## Tools Used
- MobSF
- Frida
- Kali Linux / Android testing environment

## Steps Performed
1. Loaded the mobile application package for analysis.
2. Performed static analysis using MobSF.
3. Reviewed findings related to insecure storage, permissions, and exposed application behavior.
4. Performed dynamic observation using Frida hooks.
5. Documented evidence of runtime inspection and security weakness indicators.

## Screenshot Reference
- `mobsf_report.png` – MobSF static analysis report
- `frida_hook.png` – Frida runtime hook evidence

## Log Entry
| Test ID | Vulnerability     | Severity | Target App |
|---------|-------------------|----------|------------|
| 016     | Insecure Storage  | High     | test.apk   |

## Dynamic Testing Summary 
Static analysis identified insecure handling of application data and potentially unsafe storage practices. Dynamic testing with Frida demonstrated how runtime behavior can be observed or modified, showing that weak protections may allow authentication bypass or sensitive function monitoring. Mobile apps should enforce secure storage and strong runtime defense mechanisms.

## Checklist
- [x] Performed MobSF static analysis
- [x] Reviewed findings
- [x] Performed Frida-based runtime observation
- [x] Saved screenshots as evidence

## Conclusion
This lab demonstrated how mobile applications can expose sensitive information through insecure storage and weak runtime protections. Secure coding, encryption, obfuscation, and integrity checks are important for mobile application security.
