---
layout: post
title:      "Securing Web Applications"
date:       2020-11-29 18:51:34 +0000
permalink:  securing_web_applications
---

Security is majorly important in all web applications. It must be built into the application from the ground up, and not treated as a separate component of development. There are countless numbers of breaches taking place yearly, and there is a greater need applications to be secure enough from attacks. There are many important places in web applications that need security controls. It only takes one security flaw for a hacker to succeed. It is not uncommon for only a couple hackers to breach into a large company that has many more security professionals developing security controls. 

The developers of an application should either secure these things well, or expect a damaging security breach. Although a company should never under budget for security resources, it is also important to invest wisely and not overspend. Unfortunately, many companies wait until a large breach has occurred before they decide to budget for security. Although it may be tempting, companies should not cut back on security funding.


OWASP lists the top ten most common web application security risks. They are as follows:

1. Injection
2. Broken Authentication
3. Sensitive Data Exposure
4. XML External Entities (XXE)
5. Broken Access Control
6. Security Misconfiguration
7. Cross-Site Scripting XSS
8. Insecure Deserialization
9. Using Components with Known Vulnerabilities
10. Insufficient Logging & Monitoring


Of injection attacks, SQL injection is one of the most common. Many applications use SQL as a database, and SQL injection is a powerful way to manipulate the database. A successful SQL injection attack might cause massive data leakage. For example, here is a simple command that can drop an entire database:

```
DROP DATABASE <databasename>;
```

Just these three words can delete a large amount of a company’s information. This could cause major layoffs, or even company failure because information is one of a company's most valuable asset.

Sources:
https://owasp.org/www-project-top-ten/

