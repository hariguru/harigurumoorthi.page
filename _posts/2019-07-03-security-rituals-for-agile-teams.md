---
title: Security Rituals for Agile Teams
tags: [DevOps, Agile, Security]
style: 
color: 
description: Security has always been an afterthought for agile teams. Security requirements are mostly discussed and identified during the discovery or high-level planning phase and tested at the end, leaving a vacuum during the process. This blog series brings some simple rituals for Agile Teams. 
---

Security has always been an afterthought for agile teams. One of the common premise agile teams neglect Security is because it is not an explicit part of the common agile framework. Security requirements are mostly discussed and identified during the discovery or high-level planning phase and tested at the end, leaving a vacuum during the process. This blog series brings some simple rituals that can be part of Agile and DevOps practices.

## Security Rituals
The word ritual is quite used in the context of doing religious customary observance or practices that are sacred and done with dedication. Keeping security is of prime importance need for a strong belief system among the agile teams.   
## Product Owner Security Rituals
Accentuating security needs in an Epic or a User Story has never been practiced as they are considered implicit requirements unless it, they are very specific needs like Single-Sign-On integration. Engineering teams cannot silently take care of security without product owners explicitly motivating and requiring security features. Security may remain invisible and intangible.  
### Explicit security requirements
Product Owner should articulate clearly “Why” security is of high importance in protecting Data, Systems, and People. Capturing the security requirements is a little challenging as we are not used to it. Some of the techniques that would help us  start are as follows
### Security Personas and Anti-Personas
Defining personas who try to break the system will help the team to understand the mindset. For example, defining personas like Hacker, Malware developer, organized criminal gang will help to understand the motive and incentive that would trigger to break the system

**Reference**
- [User personas for privacy and security](https://medium.com/@gusandrews/user-personas-for-privacy-and-security-a8b35ae5a63b)
- [A methodology of developing Attacker Personas ](https://www.cs.ox.ac.uk/files/4007/PID1871807.pdf)

### Attacker or Evil User Stories
Next logical progression would be to think like an attacker and create some high-level stories that would help the engineering team to address the security requirements.
*Example*
"As a hacker, I can send bad data in the content of requests, so I can access data and functions for which I'm not authorized." [Source](https://dzone.com/articles/adding-appsec-agile-security)

### SAFECode Security Stories 
SAFECode, the Software Assurance Forum for Excellence in Code, is an industry group made up of vendors like Adobe, Oracle, and Microsoft which provides guidance on software security and assurance. SAFECode provides Security Stories covering CWE/SANS Top 25 Most Dangerous Development Error List and OWASP Top 10 list. Product Owner can take advantage this list.

[SAFECode:Practical Security Stories and Security Tasks for Agile Development Environments](https://safecode.org/publication/SAFECode_Agile_Dev_Security0712.pdf)

### Threat Modeling
Threat Modeling is an interesting modeling technique that the product owner can take the help of security professionals and engineering team to identify the trust boundaries and system vulnerabilities and create stories for the team

[GOTO 2017 • Adaptive Threat Modelling • Aaron Bedra](https://www.youtube.com/watch?v=YTtO_TGV2fU)

### Using Definition of Done or Acceptance Criteria
Another way to list security verification criteria is by using Acceptance Criteria as part of User Stories. Good start for the web application is by using the OWASP Application Security Verification Standard (ASVS) checklist.

[OWASP Application Security Verification Standard v3.0](https://www.owasp.org/images/6/67/OWASPApplicationSecurityVerificationStandard3.0.pdf)

In the part, we will see how security rituals for Engineering Team.




