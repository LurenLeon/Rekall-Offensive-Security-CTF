


|**Vulnerability 8**|**Findings**|
| :-: | :-: |
|**Title**|Open Source Exposed Data|
|**Type (Web app / Linux OS / WIndows OS)**|<p>Linux OS</p><p></p>|
|**Risk Rating**|High|
|**Description**|Found at DomainDossier on centralops.net. Utilized an open-source intelligence (OSINT) to find where sensitive info was exposed in the WHOIS data.|
|**Images**|<p>![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.001.png)</p><p>Flag 1: h8s692hskasd </p>|
|**Affected Hosts**|TotalRekall.xyz|
|**Remediation** |Domains must be registered privately to avoid sensitive information from being exposed in domain registries.|


|**Vulnerability 9**|**Findings**|
| :-: | :-: |
|**Title**|Pinging |
|**Type (Web app / Linux OS / WIndows OS)**|<p>Linux OS</p><p></p>|
|**Risk Rating**|Low|
|**Description**|The IP is from totalrekall.xyz which is the flag for this.|
|**Images**|<p>Ping totalrekall.xyz</p><p>![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.002.png)![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.003.png)</p><p>Flag 2: 15.197.148.33</p>|
|**Affected Hosts**|TotalRekall.xyz|
|**Remediation** |Have servers limit the info provided when responding to network diagnostic commands, such as ping.|






|**Vulnerability 10**|**Findings**|
| :-: | :-: |
|**Title**|SSL and CRT Information|
|**Type (Web app / Linux OS / WIndows OS)**|Linux OS|
|**Risk Rating**|Medium|
|**Description**|Found at crt.sh. Open source data found through SSL info and crt.sh. This subdomain is exposed to the public and could provide attackers with information for potential attacks.|
|**Images**|![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.004.png)Flag 3: s7euwehd.totalrekall.xyz|
|**Affected Hosts**|TotalRekall.xyz|
|**Remediation** |Limit the publication of DNS records.|


|**Vulnerability 11**|**Findings**|
| :-: | :-: |
|**Title**|NMap Scan|
|**Type (Web app / Linux OS / WIndows OS)**|Linux OS|
|**Risk Rating**|Critical|
|**Description**|We nmap scan 192.168.13.0/24 and find 5 hosts|
|**Images**|![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.005.png)Flag 4: 5 hosts (the flag is 5)|
|**Affected Hosts**|<p>192\.168.13.10</p><p>192\.168.13.11</p><p>192\.168.13.12</p><p>192\.168.13.13</p><p>192\.168.13.14</p>|
|**Remediation** |IP blocking for unauthorized users|



|**Vulnerability 12**|**Findings**|
| :-: | :-: |
|**Title**|Aggressive Nmap Scan|
|**Type (Web app / Linux OS / WIndows OS)**|Linux OS|
|**Risk Rating**|Critical|
|**Description**|Below we can see that Drupal is the vulnerability for 192.168.13.13 (The flag is 192.168.13.13). Ran an aggressive Nmap scan to discover which host was running Drupal.|
|**Images**|<p>![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.006.png)</p><p>Flag 5: 192.168.13.13</p>|
|**Affected Hosts**|192\.168.13.13|
|**Remediation** |Block Probes|



|**Vulnerability 13**|**Findings**|
| :-: | :-: |
|**Title**|Nessus Scan|
|**Type (Web app / Linux OS / WIndows OS)**|Linux OS|
|**Risk Rating**|Medium|
|**Description**|The ID of the vulnerability from the Nessus scan for 192.168.13.12 is 97610.|
|**Images**|<p>![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.007.png)![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.008.png)</p><p>Flag 6: 97610 </p>|
|**Affected Hosts**|192\.168.13.12|
|**Remediation** |Update and patch software on a regular basis. Always monitor for new vulnerabilities.|



|**Vulnerability 14**|**Findings**|
| :-: | :-: |
|**Title**|Apache Struts 2.3.5-2.3.31/2.5x<2.5.10.1 Jakarta Multipart parser RCE (remote)|
|**Type (Web app / Linux OS / WIndows OS)**|Linux OS|
|**Risk Rating**|Critical|
|**Description**|We ran a Nessus scan, found that Apache Tomcat Remote Code Execution is a vulnerability. RCE exploits can be used for attackers to run programs and exfiltrate data.|
|**Images**|<p>![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.009.png)![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.010.png)![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.011.png)![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.012.png)</p><p>Flag 7: 8ks6sbhss</p>|
|**Affected Hosts**|192\.168.13.10 |
|**Remediation** |Upgrade Apache Struts|



|**Vulnerability 15** |**Findings**|
| :-: | :-: |
|**Title**|Nessus Scan Struts Vulnerability|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|High|
|**Description**|We use a struts vulnerability, found with Nessus scan, used metasploit to exploit struts2\_content\_type\_ognl|
|**Images**|<p>![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.013.png)![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.014.png)![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.015.png)![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.016.png)![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.017.png)</p><p>Flag 10: wjasdufsdkg </p>|
|**Affected Hosts**|192\.168.13.12|
|**Remediation** |Update Apache|



|**Vulnerability 16**|**Findings**|
| :-: | :-: |
|**Title**|Drupal CVE-2019-6340|
|**Type (Web app / Linux OS / WIndows OS)**|Linux OS|
|**Risk Rating**|High|
|**Description**|Exploited drupal\_retws\_unserialize on metasploit, run command getiud to attain username on Meterpreter session. The Drupal vulnerability CVE-2019-6340 can be exploited to attain unauthorized access to user data.|
|**Images**|<p>![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.018.png)</p><p>Flag 11: www-data</p>|
|**Affected Hosts**|192\.168.13.13|
|**Remediation** |Update Drupal on a regular basis.|







|**Vulnerability 17**|**Findings**|
| :-: | :-: |
|**Title**|CVE-2019-14287|
|**Type (Web app / Linux OS / WIndows OS)**|Linux OS|
|**Risk Rating**||
|**Description**|Ssh into the server, use the password ‘alice’ and performed privilege escalation to obtain the flag using a sudo vulnerability (CVE-2019-14287): sudo-u#-1 cat /root/flag12.txt. |
|**Images**|<p>![](Aspose.Words.533d53bb-66b5-44fc-9c52-d39af05e73a7.019.png)</p><p>Flag 12: d7sdfksdf384</p>|
|**Affected Hosts**|192\.168.13.14|
|**Remediation** |Update sudo on a regular basis, sudo permissions restricted, always use secure passwords, never share or post passwords.|


