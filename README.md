# Rekall-Offensive-Security-CTF

## Introduction

In accordance with Rekall policies, our organization conducts external and internal penetration tests of its networks and systems throughout the year. The purpose of this engagement was to assess the networks’ and systems’ security and identify potential security flaws by utilizing industry-accepted testing methodology and best practices.

For the testing, we focused on the following:

- Attempting to determine system-level vulnerabilities with no prior knowledge of the environment.
- Attempting to exploit vulnerabilities found and access confidential information.
- Documenting and reporting on all findings.

All tests took into consideration the actual business processes, providing a realistic picture of exposure levels to online hackers.

### Assessment Objective

The primary goal of this assessment was to analyze security flaws in Rekall’s web applications, networks, and systems. The assessment aimed to identify exploitable vulnerabilities and provide actionable recommendations for remediation.

Rekall's defined objectives:
- Find and exfiltrate any sensitive information within the domain.
- Escalate privileges.
- Compromise several machines.

## Penetration Testing Methodology

### Reconnaissance

We begin assessments by checking for any passive (open source) data that may assist the assessors. If internal, the assessment team will perform active recon using tools such as Nmap and Bloodhound.

### Identification of Vulnerabilities and Services

We use custom, private, and public tools such as Metasploit, hashcat, and Nmap to gain perspective on network security. These methods provide Rekall with an understanding of risks and strengths within its information systems.

### Vulnerability Exploitation

We manually test each identified vulnerability and use automated tools to exploit these issues, defining exploitation as any action that gives unauthorized access to systems or sensitive data.

### Reporting

Once exploitation is completed, the assessment team writes the report, the final deliverable to the customer.

# Scope

Prior to any assessment activities, Rekall and the assessment team identify targeted systems with a defined range or list of network IP addresses. In-scope and excluded IP addresses and ranges are listed below.

## Executive Summary of Findings

### Grading Methodology

Each finding was classified according to its severity, reflecting the risk each vulnerability may pose to business processes.

- **Critical**: Immediate threat to key business processes.
- **High**: Indirect threat to key business processes/threat to secondary business processes.
- **Medium**: Indirect or partial threat to business processes.
- **Low**: No direct threat exists; vulnerability may be leveraged with other vulnerabilities.
- Informational: No threat; however, data may be used in a future attack.

### Summary of Strengths

While the assessment team found vulnerabilities, they also recognized several strengths within Rekall’s environment:

- Robust protection in Web Application input fields against basic XSS exploits.
- Unsuccessful attempts at SQL injections on the web page.
- Enhanced defenses against exploits like Local File inclusion and XSS scripting.
- Effective input validation in many input fields.

### Summary of Weaknesses

The team found critical vulnerabilities that should be immediately addressed:

- Web app vulnerabilities: susceptible to XSS scripting, Local File Inclusion, and command injections.
- Sensitive data exposure: Linux and Windows machines exhibit cases of exposed data.
- Network vulnerabilities: Basic nmap scans reveal several open ports.
- Old vulnerabilities: Windows and Linux machines harbor outdated vulnerabilities.
- Open source intelligence findings: WHOIS data and other information obtained through open-source tools can be leveraged by adversaries.
- Credential compromise: Using kiwi, critical user credentials were retrieved and passwords cracked.

## Summary Vulnerability Overview

| Vulnerability                                          | Severity  |
| ------------------------------------------------------ | --------- |
| Cross Site Scripting                                   | Critical  |
| Local File Inclusion                                   | Critical  |
| Command Injection                                      | Critical  |
| Apache Struts 2.3.5-2.3.31/2.5x<2.5.10.1 Jakarta Multipart parser RCE (remote) | Critical  |
| Exposed data on totalrekall Github                      | High      |
| SLMail Pop3                                             | Medium    |
| Exclusion Standard Settings Exposure                    | Low      |

The following summary tables represent an overview of the assessment findings for this penetration test:

| Scan Type         | Total                                                                                                                                                   |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Hosts             | 34.102.136.180 – totalrekall.xyz 192.168.13.10 - Linux 192.168.13.11 - Linux 192.168.13.12 - Linux 192.168.13.13 - Linux 192.168.13.14 - Linux 192.168.13.1 – Linux 172.22.117.20 – Windows10 172.22.117.10 – Windows Domain Controller 172.22.117.100 – Windows host |
| Ports             | 80 (HTTP) 21(FTP), 25(SMTP), 110 (POP3), 135 (RPC), 8009 (TCP), 8080                                                                                    |

| Exploitation Risk | Total |
| ------------------ | ----- |
| Critical           | 15    |
| High               | 4     |
| Medium             | 2     |
| Low                | 2     |


## Linux Vulnerabilities 
**[Linux CTF Vulnerabilities](https://github.com/LurenLeon/Rekall-Offensive-Security-CTF/blob/main/Linux/CTF%20Day%202_%20Linux/CTF%20Day%202_%20Linux.md)**

## Windows Vulnerabilities
**[Windows Vulnerabilities](https://github.com/LurenLeon/Rekall-Offensive-Security-CTF/blob/main/Windows/CTF%20Day%203_%20Windows%20Servers/CTF%20Day%203.md)**

## Web App Vulnerabilities 

