# Cbr540-penetration-report-host50
Penetration test against IP 50.79.107.78 conducted as part of CBR-540 coursework. Includes vulnerability discovery, exploitation (Metasploit, Nmap, vsftpd backdoor), and remediation recommendations.
# Host 50 Penetration Testing Report

## 🛡️ Overview
This repository contains a full penetration test conducted against IP address `50.79.107.78` as part of the CBR-540-R course. The goal was to identify vulnerabilities, exploit weaknesses, and document security recommendations.

## 🔧 Tools Used
- **Nmap** – Port scanning and service enumeration
- **Metasploit** – Exploitation and post-exploitation
- **Nessus** – Vulnerability scanning
- **Telnet Client** – Service testing
- **Linux (Kali)** – Recon and analysis environment

## 🚨 Key Exploits & Findings
- **rlogin Misconfiguration** – Allowed unauthenticated root access
- **vsftpd 2.3.4 Backdoor** – Opened unauthorized shell on port 6200
- **Insecure Telnet Banner** – Exposed OS details
- **Multiple SSL/TLS Weaknesses** – Including POODLE, SWEET32, and RC4
- **Apache Tomcat Vulnerabilities** – Default files and outdated version

## 📄 Report Contents
- Full PDF Report: [`Penetration_Testing_Report_for_Host_50.pdf`](./report/Penetration_Testing_Report_for_Host_50.pdf)
- Vulnerability descriptions
- Exploit steps with Metasploit
- Post-exploitation findings (captured flags, user accounts, etc.)
- Security recommendations and hardening guidelines

## 📌 Recommendations Summary
- Disable insecure services (rlogin, Telnet, FTP)
- Patch outdated software (Apache Tomcat, OpenSSL, vsftpd)
- Enforce strong access controls and MFA
- Use SSH and secure protocols only

## 👨‍💻 Author
**Zion Spearman**  
CBR-540-R – Instructor: Thomas Dodds  
December 2024
