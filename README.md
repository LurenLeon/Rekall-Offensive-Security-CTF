# Rekall-Offensive-Security-CTF

## <a name="_nb9r73bykkqu"></a>Introduction

<a name="_tyjcwt"></a>In accordance with Rekall policies, our organization conducts external and internal penetration tests of its networks and systems throughout the year. The purpose of this engagement was to assess the networks’ and systems’ security and identify potential security flaws by utilizing industry-accepted testing methodology and best practices.

For the testing, we focused on the following:

- Attempting to determine what system-level vulnerabilities could be discovered and exploited with no prior knowledge of the environment or notification to administrators.
- Attempting to exploit vulnerabilities found and access confidential information that may be stored on systems.
- Documenting and reporting on all findings.

All tests took into consideration the actual business processes implemented by the systems and their potential threats; therefore, the results of this assessment reflect a realistic picture of the actual exposure levels to online hackers. This document contains the results of that assessment.

### <a name="_3dy6vkm"></a>**Assessment Objective**

<a name="_1t3h5sf"></a>The primary goal of this assessment was to provide an analysis of security flaws present in Rekall’s web applications, networks, and systems. This assessment was conducted to identify exploitable vulnerabilities and provide actionable recommendations on how to remediate the vulnerabilities to provide a greater level of security for the environment.

We used our proven vulnerability testing methodology to assess all relevant web applications, networks, and systems in scope. 

Rekall has outlined the following objectives:

Table 1: Defined Objectives


|**Objective**|
| :-: |
|Find and exfiltrate any sensitive information within the domain.|
|Escalate privileges.|
|Compromise several machines.|

## <a name="_tgl1cd57dphe"></a>Penetration Testing Methodology

### <a name="_17dp8vu"></a>**Reconnaissance**
### <a name="_3lzx45vd2jl6"></a>
We begin assessments by checking for any passive (open source) data that may assist the assessors with their tasks. If internal, the assessment team will perform active recon using tools such as Nmap and Bloodhound.

### <a name="_3rdcrjn"></a>**Identification of Vulnerabilities and Services**

We use custom, private, and public tools such as Metasploit, hashcat, and Nmap to gain perspective of the network security from a hacker’s point of view. These methods provide Rekall with an understanding of the risks that threaten its information, and also the strengths and weaknesses of the current controls protecting those systems. The results were achieved by mapping the network architecture, identifying hosts and services, enumerating network and system-level vulnerabilities, attempting to discover unexpected hosts within the environment, and eliminating false positives that might have arisen from scanning. 

### <a name="_26in1rg"></a>**Vulnerability Exploitation**

Our normal process is to both manually test each identified vulnerability and use automated tools to exploit these issues. Exploitation of a vulnerability is defined as any action we perform that gives us unauthorized access to the system or the sensitive data. 

### <a name="_lnxbz9"></a>**Reporting**

Once exploitation is completed and the assessors have completed their objectives, or have done everything possible within the allotted time, the assessment team writes the report, which is the final deliverable to the customer.

# <a name="_506wczneb2re"></a>
## <a name="_zf3a4holuf89"></a>Scope

Prior to any assessment activities, Rekall and the assessment team will identify targeted systems with a defined range or list of network IP addresses. The assessment team will work directly with the Rekall POC to determine which network ranges are in-scope for the scheduled assessment. 

It is Rekall’s responsibility to ensure that IP addresses identified as in-scope are actually controlled by Rekall and are hosted in Rekall-owned facilities (i.e., are not hosted by an external organization). In-scope and excluded IP addresses and ranges are listed below. 


## <a name="_x5kpi12umwq3"></a>Executive Summary of Findings
##
### <a name="_2jxsxqh"></a><a name="_z337ya"></a>**Grading Methodology**

Each finding was classified according to its severity, reflecting the risk each such vulnerability may pose to the business processes implemented by the application, based on the following criteria:

**Critical**:	 Immediate threat to key business processes.

**High**:		 Indirect threat to key business processes/threat to secondary business processes.

**Medium**:	 Indirect or partial threat to business processes. 

**Low**:		 No direct threat exists; vulnerability may be leveraged with other vulnerabilities.

Informational:    No threat; however, it is data that may be used in a future attack.

As the following grid shows, each threat is assessed in terms of both its potential impact on the business and the likelihood of exploitation:

### <a name="_nntf0x9u7qng"></a>**Summary of Strengths**

While the assessment team was successful in finding several vulnerabilities, the team also recognized several strengths within Rekall’s environment. These positives highlight the effective countermeasures and defenses that successfully prevented, detected, or denied an attack technique or tactic from occurring. 

- Robust protection in Web Application input fields against basic XSS exploits 
- Unsuccessful attempts at SQL injections on the web page 
- Enhanced defenses against exploits like Local File inclusion and XSS scripting 
- Effective input validation in many input fields

### <a name="_1y810tw"></a>**Summary of Weaknesses**

We successfully found several critical vulnerabilities that should be immediately addressed in order to prevent an adversary from compromising the network. These findings are not specific to a software version but are more general and systemic vulnerabilities.

- Web app vulnerabilities: susceptible to XSS scripting, Local File Inclusion, and command injections, allowing threat actors easy access to sensitive data and potential upload of malicious scripts on Rekall’s servers.
- Sensitive data exposure: Linux and Windows machines exhibit cases of exposed data, making important information easily accessible to potential threat actors who compromise the system.
- Network vulnerabilities: Basic nmap scans reveal several open ports, exposing potential weaknesses in Rekall’s network.
- Old vulnerabilities: Windows and Linux machines harbor outdated vulnerabilities like Shellshock, SLMail pop3d, and Apache Tomcat Remote Code Execution.
- Open source intelligence findings: WHOIS data and other information obtained through open-source tools can be leveraged by adversaries for network scanning and vulnerability discovery.
- Credential compromise: Using kiwi, critical user credentials were retrieved and passwords cracked, posing a significant security risk.

## <a name="_tr5kilpcz7z8"></a>Summary Vulnerability Overview



|**Vulnerability**|**Severity**|
| :-: | :-: |
|Cross Site Scripting|**Critical**|
|Local File Inclusion|**Critical**|
|Command Injection|**Critical**|
|Apache Struts 2.3.5-2.3.31/2.5x<2.5.10.1 Jakarta Multipart parser RCE (remote)|**Critical**|
|Exposed data on totalrekall Github|**High**|
|SLMail Pop3|**Medium**|
|Exclusion Standard Settings Exposure|**Low**|


The following summary tables represent an overview of the assessment findings for this penetration test:


|**Scan Type**|**Total**|
| :-: | :-: |
|Hosts|34\.102.136.180 – totalrekall.xyz 192.168.13.10 - Linux 192.168.13.11 - Linux 192.168.13.12 - Linux 192.168.13.13 - Linux 192.168.13.14 - Linux 192.168.13.1 – Linux 172.22.117.20 – Windows10 172.22.117.10 – Windows Domain Controller 172.22.117.100 – Windows host|
|Ports|80 (HTTP) 21(FTP), 25(SMTP), 110 (POP3), 135 (RPC), 8009 (TCP), 8080|


|**Exploitation Risk**|**Total**|
| :-: | :-: |
|**Critical**|15|
|**High**|4|
|**Medium**|2|
|**Low**|2|

