


|**Vulnerability 25**|**Findings**|
| :-: | :-: |
|**Title**|Exclusion Standard Settings|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Low|
|**Description**|Added “robots.txt” at the end of the IP address. This revealed the robots exclusion standard settings for the website. Attackers can use this info to find targets for potential exploits.|
|**Images**|![](Aspose.Words.ee139356-0e1e-425a-99b4-441326b284f3.001.png)|
|**Affected Hosts**|TotalRekall.xyz|
|**Remediation** |Utilize Noindex for pages that need to be private (while publicly accessible)|



|**Vulnerability 26**|**Findings**|
| :-: | :-: |
|**Title**|Command Injection Type|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|On /Networking.php we can access the vendors.txt page. Using this we can input “[www.example.com](http://www.example.com); cat vendors.txt” inside the search bar intended for DNS check images.|
|**Images**|![](Aspose.Words.ee139356-0e1e-425a-99b4-441326b284f3.002.png)![](Aspose.Words.ee139356-0e1e-425a-99b4-441326b284f3.003.png)|
|**Affected Hosts**|TotalRekall.xyz|
|**Remediation** |Implement input validation for unintended access|





|**Vulnerability 27**|**Findings**|
| :-: | :-: |
|**Title**|Command Injection Type|
|**Type (Web app / Linux OS / WIndows OS)**|Web App|
|**Risk Rating**|Critical|
|**Description**|On /Networking.php we can access the vendors.txt page. Using this we can input “splunk” inside the search bar intended for DNS check images.|
|**Images**|![](Aspose.Words.ee139356-0e1e-425a-99b4-441326b284f3.004.png)|
|**Affected Hosts**|TotalRekall.xyz|
|**Remediation** |Implement input validation for unintended access|


