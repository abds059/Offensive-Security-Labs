# Offensive Security Home Lab – Metasploitable2 VAPT

## Overview
This repository documents a complete Vulnerability Assessment and Penetration
Testing (VAPT) exercise performed on the Metasploitable2 virtual machine in a
controlled lab environment. The objective was to practice the full penetration
testing lifecycle, from reconnaissance to post-exploitation reporting.

---

## Lab Environment
- Attacker Machine: Kali Linux
- Target Machine: Metasploitable2
- Network Configuration: Host-only / NAT
- Scope: Internal network penetration test

---

## Methodology
The assessment followed a structured penetration testing approach:

1. Reconnaissance
2. Vulnerability Identification
3. Exploitation
4. Privilege Escalation
5. Post-Exploitation
6. Reporting & Risk Assessment

---

## Reconnaissance
Initial reconnaissance was performed to identify open ports, running services,
and exposed web applications on the target system.

- Network and service discovery using Nmap
- Web application enumeration
- Identification of vulnerable services

Detailed findings:  
[Reconnaissance](./Reconnaisance/)

---

## Exploitation

### Web Application Exploitation
Multiple web vulnerabilities were identified and exploited, including SQL
Injection, Cross-Site Scripting (XSS), and weak authentication mechanisms.

- SQL Injection (DVWA)  
  [Exploitation/Web/DVWA/SQL-Injection.md](./Exploitation/Web/DVWA/SQL%20Injection.md)

- Cross-Site Scripting (DVWA)  
  [Exploitation/Web/DVWA/XSS.md](./Exploitation/Web/DVWA/XSS.md)

- Brute Force Attack  
  [Exploitation/Web/DVWA/Brute-Force.md](./Exploitation/Web/DVWA/Brute-Force.md)

---

## Privilege Escalation
Post-exploitation enumeration was conducted to identify misconfigurations that
allowed privilege escalation to higher-privileged users, including root.

Details:  
[Privilege Escalation](./Privelege%20Escalation/)

---

## Post-Exploitation
After gaining elevated privileges, post-exploitation activities were performed
to evaluate impact, persistence, and data exposure.

---

## Reporting & Risk Assessment
Each identified vulnerability was documented with proof of concept, impact,
severity, and mitigation recommendations.

Details:  
[Reporting](./Reporting/)

---

## Disclaimer
This project was conducted in a controlled lab environment for educational
purposes only. No unauthorized testing was performed.
