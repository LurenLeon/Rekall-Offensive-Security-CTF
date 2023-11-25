CTF Day 1: 


|**Vulnerability  18**|**Findings**|
| :-: | :-: |
|**Title**|Cross Site Scripting XSS|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|Using <script>alert(document.cookie)</script> we are able to attain the flag. We can insert scripts into the input fields and bypass the input validation settings. By doing so, we could potentially insert scripts that redirect users to a spoofed web page to steal their data.|
|**Images**|![](Aspose.Words.10c5b413-03ca-4951-8f54-2a9d65c1cc3d.001.png)|
|**Affected Hosts**|Totalrekall.xyz|
|**Remediation** |Output Encoding, HTML Sanitization |



|**Vulnerability 19**|**Findings**|
| :-: | :-: |
|**Title**|Cross Site Scripting XSS #2|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|<script> is filtered out so we use <scr<script>ipt> to make a full <script> show up on the code.  Therefore we use scrscriptipt. We can insert scripts into the input fields and bypass the input validation settings. By doing so, we could potentially insert scripts that redirect users to a spoofed web page to steal their data. In addition, it could be used to gain unauthorized entry.|
|**Images**|![](Aspose.Words.10c5b413-03ca-4951-8f54-2a9d65c1cc3d.002.png)|
|**Affected Hosts**|Totalrekall.xyz|
|**Remediation** |Output Encoding, HTML Sanitization |



|**Vulnerability 20**|**Findings**|
| :-: | :-: |
|**Title**|Cross Site Scripting XSS 3|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|Using <script>alert(“hi)</script> we got a pop-up to attain flag 3. We can insert scripts into the input fields and bypass the input validation settings. By doing so, we could potentially insert scripts that redirect users to a spoofed web page to steal their data. In addition, it could be used to gain unauthorized entry.|
|**Images**|![](Aspose.Words.10c5b413-03ca-4951-8f54-2a9d65c1cc3d.003.png)|
|**Affected Hosts**|Totalrekall.xyz|
|**Remediation** |Output Encoding, HTML Sanitization |



|**Vulnerability 21**|**Findings**|
| :-: | :-: |
|**Title**|Local File Inclusion|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|Created a PHP script file and uploaded it into the upload file of the Memory Planner section. Allowing .php files to be uploaded can result in malicious scripts being ran again the database to modify/delete data.|
|**Images**|![](Aspose.Words.10c5b413-03ca-4951-8f54-2a9d65c1cc3d.004.png)|
|**Affected Hosts**|TotalRekall.xyz|
|**Remediation** |Restrict certain file types from being uploaded|



|**Vulnerability 22**|**Findings**|
| :-: | :-: |
|**Title**|Local File Inclusion #2|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|Created a PHP script file and uploaded it into the upload file of the Memory Planner section. Allowing .php files to be uploaded can result in malicious scripts being ran again the database to modify/delete data.|
|**Images**|![](Aspose.Words.10c5b413-03ca-4951-8f54-2a9d65c1cc3d.005.png)|
|**Affected Hosts**|TotalRekall.xyz|
|**Remediation** |Restrict certain file types from being uploaded|



|**Vulnerability 23**|**Findings**|
| :-: | :-: |
|**Title**|SQL Injection|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|Using a basic SQL Injection: ' or '1'='1   ' or '1'='1 for user and pass we’re able to log in and capture the flag.|
|**Images**|<p>![](Aspose.Words.10c5b413-03ca-4951-8f54-2a9d65c1cc3d.006.png)</p><p>Flag 7: bcs92sjsk233</p>|
|**Affected Hosts**|TotalRekall.xyz |
|**Remediation** |Input validation|



|**Vulnerability 24**|**Findings**|
| :-: | :-: |
|**Title**|Command Injection|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|Found username and password within HTML file of user “dougquaid” and password “kuato”. We used these credentials to log in as an administrator and found the location of more sensitive data in vendors.txt. This log-in is also vulnerable to SQL injections.|
|**Images**|![](Aspose.Words.10c5b413-03ca-4951-8f54-2a9d65c1cc3d.007.png)![](Aspose.Words.10c5b413-03ca-4951-8f54-2a9d65c1cc3d.008.png)|
|**Affected Hosts**|TotalRekall.xyz|
|**Remediation** |Delete sensitive data from files, limit use of command execution functions.|

