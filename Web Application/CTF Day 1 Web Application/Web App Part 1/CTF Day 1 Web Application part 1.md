


|**Vulnerability  18**|**Findings**|
| :-: | :-: |
|**Title**|Cross Site Scripting XSS|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|Using <script>alert(document.cookie)</script> we are able to attain the flag. We can insert scripts into the input fields and bypass the input validation settings. By doing so, we could potentially insert scripts that redirect users to a spoofed web page to steal their data.|
|**Images**|![](Aspose.Words.ade8f726-6b6e-4fb2-b940-1eb6b8cf8598.001.png)|
|**Affected Hosts**|Totalrekall.xyz|
|**Remediation** |Output Encoding, HTML Sanitization |



|**Vulnerability 19**|**Findings**|
| :-: | :-: |
|**Title**|Cross Site Scripting XSS #2|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|<script> is filtered out so we use <scr<script>ipt> to make a full <script> show up on the code.  Therefore we use scrscriptipt. We can insert scripts into the input fields and bypass the input validation settings. By doing so, we could potentially insert scripts that redirect users to a spoofed web page to steal their data. In addition, it could be used to gain unauthorized entry.|
|**Images**|![](Aspose.Words.ade8f726-6b6e-4fb2-b940-1eb6b8cf8598.002.png)|
|**Affected Hosts**|Totalrekall.xyz|
|**Remediation** |Output Encoding, HTML Sanitization |



|**Vulnerability 20**|**Findings**|
| :-: | :-: |
|**Title**|Cross Site Scripting XSS 3|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|Using <script>alert(“hi)</script> we got a pop-up to attain flag 3. We can insert scripts into the input fields and bypass the input validation settings. By doing so, we could potentially insert scripts that redirect users to a spoofed web page to steal their data. In addition, it could be used to gain unauthorized entry.|
|**Images**|![](Aspose.Words.ade8f726-6b6e-4fb2-b940-1eb6b8cf8598.003.png)|
|**Affected Hosts**|Totalrekall.xyz|
|**Remediation** |Output Encoding, HTML Sanitization |



|**Vulnerability 21**|**Findings**|
| :-: | :-: |
|**Title**|Local File Inclusion|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|Created a PHP script file and uploaded it into the upload file of the Memory Planner section. Allowing .php files to be uploaded can result in malicious scripts being ran again the database to modify/delete data.|
|**Images**|![](Aspose.Words.ade8f726-6b6e-4fb2-b940-1eb6b8cf8598.004.png)|
|**Affected Hosts**|TotalRekall.xyz|
|**Remediation** |Restrict certain file types from being uploaded|



|**Vulnerability 22**|**Findings**|
| :-: | :-: |
|**Title**|Local File Inclusion #2|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|Created a PHP script file and uploaded it into the upload file of the Memory Planner section. Allowing .php files to be uploaded can result in malicious scripts being ran again the database to modify/delete data.|
|**Images**|![](Aspose.Words.ade8f726-6b6e-4fb2-b940-1eb6b8cf8598.005.png)|
|**Affected Hosts**|TotalRekall.xyz|
|**Remediation** |Restrict certain file types from being uploaded|


﻿


|**Vulnerability 23**|**Findings**|
| :-: | :-: |
|**Title**|SQL Injection|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|Using a basic SQL Injection: ' or '1'='1   ' or '1'='1 for user and pass we’re able to log in and capture the flag.|
|**Images**|![](Aspose.Words.0c858bcc-1e54-44c0-86c4-08c30823b767.001.png)|
|**Affected Hosts**|TotalRekall.xyz|
|**Remediation** |Input validation|




