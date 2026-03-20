# API Security Testing Lab

## Objective
To perform API security testing and identify common vulnerabilities such as Broken Object Level Authorization (BOLA) through request interception and manipulation.

## Target Details
- **Attacker IP:** 192.168.56.103
- **Target IP:** 192.168.56.102

## Tools Used
- Burp Suite
- Postman
- Kali Linux

## Steps Performed
1. Opened the target web/API application.
2. Configured Burp Suite proxy for request interception.
3. Captured API requests using Burp Suite.
4. Modified parameters to check whether unauthorized access to other resources was possible.
5. Observed application response after changing object identifiers.
6. Documented evidence of authorization weakness.

## Screenshot Reference
- `api_burp_intercept.png` – API request intercepted in Burp Suite
- `bola_result.png` – Evidence of modified request and unauthorized access

## Log Entry
| Test ID | Vulnerability | Severity | Target Endpoint |
|---------|---------------|----------|-----------------|
| 008     | BOLA          | Critical | /api/users      |
| 009     | GraphQL Injection | High | /graphql        |

## API Test Summary (50 words)
API testing revealed weak authorization controls, allowing requests to be modified for access to unauthorized data. By changing object identifiers, the application returned information beyond the intended user scope. This indicates Broken Object Level Authorization and shows that access validation must be enforced server-side for every request.

## Checklist
- [x] Enumerated API behavior
- [x] Intercepted requests using Burp Suite
- [x] Modified identifiers for BOLA testing
- [x] Documented findings with screenshots

## Conclusion
This lab demonstrated how insecure access control in APIs can expose sensitive information. Proper authorization checks and input validation are necessary to prevent such flaws in real-world applications.
