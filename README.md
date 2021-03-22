# security-test
[![](https://img.shields.io/badge/license-Siemens%20Inner%20Source-blue.svg)](https://code.siemens.com/siemens/code/blob/master/LICENSE.md)

# Security Testing for Data-API

Zaptest Open API which conatins all API's Which include 

# Online data
# Historical Data
# Meta Data

# what is security Testing?
SECURITY TESTING is a type of Software Testing that uncovers vulnerabilities, threats, risks in a software application and prevents malicious attacks from intruders. 
The purpose of Security Tests is to identify all possible loopholes and weaknesses of the software system which might result in a loss of information, revenue, repute at the hands of the employees or outsiders of the Organization.

# Types of Security Testing 

There are seven main types of security testing as per Open Source Security Testing methodology manual. They are explained as follows:

# Vulnerability Scanning: 
This is done through automated software to scan a system against known vulnerability signatures.

# Security Scanning: 
It involves identifying network and system weaknesses, and later provides solutions for reducing these risks. This scanning can be performed for both Manual and Automated scanning.

# Penetration testing: 
This kind of testing simulates an attack from a malicious hacker. This testing involves analysis of a particular system to check for potential vulnerabilities to an external hacking attempt.

# Risk Assessment: 
This testing involves analysis of security risks observed in the organization. Risks are classified as  Low, Medium and High. This testing recommends controls and measures to reduce the risk.

# Security Auditing: 
This is an internal inspection of Applications and Operating systems for security flaws. An audit can also be done via line by line inspection of code

# Ethical hacking: 
It's hacking an Organization Software systems. Unlike malicious hackers, who steal for their own gains, the intent is to expose security flaws in the system.

# Posture Assessment: 
This combines Security scanning, Ethical Hacking and Risk Assessments to show an overall security posture of an organization.

# How 
- Perform security scanning of APIs using ZAP from the command line.
- This allows you to easily automate the scanning of your APIs.
- Following the approach taken by the Baseline Scan we have introduced a new API scanning script which has only one dependency – Docker.
- You don’t need to install either ZAP or Java.
- The script, zap-api-scan.py is included in the Weekly and Live ZAP Docker images, it will also be included in the next Stable image.

#To use the API scanning script you just need to use the commands:
docker pull owasp/zap2docker-weekly  
docker run -t owasp/zap2docker-weekly zap-api-scan.py -t \  
    https://www.example.com/openapi.json -f openapi  

# Test Report 

->If you run the ZAP Test  through Docker command line in local , check the HTML report
-> if your the security testing through Gitlab runner , check the HTML report under artifacts 


## License
Code and documentation copyright 2017 Siemens AG.
See [LICENSE.md](LICENSE.md).


## Maintainer
Chakravarthi Behara
