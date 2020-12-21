---
layout: post
title:      "Web Application Attacks"
date:       2020-12-20 18:01:30 -0500
permalink:  web_application_attacks
---


Introduction

There are many known ways for attacks exploit a web application. New strategies are constantly being developed, and large breaches are being executed by attackers worldwide. In fact, “The 2020 Verizon Data Breach Investigations Report (DBIR) confirms that this is the case: 43% of data breaches are tied to web application vulnerabilities—which more than doubled year over year” (Spencer, 2020). Protecting against even a single type of attack can be difficult - so protecting against many types of attacks can be much more difficult. There are currently many advanced tools for many types of attacks, and they are quickly growing in features. Some of the most dangerous web application attacks include SQL injection, cross-site scripting, command injection, and cross-site request forgery. 
	
Method: SQL Injection

SQL Injection is a very common type of web application attack. Injection attacks are listed as the number one web application security risk, and SQL injection is one of the most common type of injection attacks. SQL is usually used to manipulate data in a database and is a very common language used by developers. SQL injection works by adding malicious SQL code to the target database. This gives attackers strong control over the target database. The following is an example of a SQL injection attack:
	SELECT * FROM tablename WHERE UserID= 2302
	becomes the following with a simple SQL injection attack:
	SELECT * FROM tablename WHERE UserID= 2302 OR 1=1”  (Gregg & Santos, 2020)
	The “OR 1=1” was maliciously added by the attacker. It will always evaluate to true, so the query will return the results of the query, ignoring the requirement in the WHERE clause of the UserID of 2302.
	
SQL Injection Tools
BSQL hacker - “a nice SQL injection tool that helps you perform a SQL injection attack against web applications. This tool is for those who want an automatic SQL injection tool. It is especially made for Blind SQL injection. This tool is fast and performs a multi-threaded attack for better and faster results.”
SQLMap - “the open source SQL injection tool and most popular among all SQL injection tools available. This tool makes it easy to exploit the SQL injection vulnerability of a web application and take over the database server. It comes with a powerful detection engine which can easily detect most of the SQL injection related vulnerabilities.”
SQLninja - “a SQL injection tool that exploits web applications that use a SQL server as a database server. This tool may not find the injection place at first. But if it is discovered, it can easily automate the exploitation process and extract the information from the database server.”
Safe3 SQL injector - “is another powerful but easy to use SQL injection tool. Like other SQL injection tools, it also makes the SQL injection process automatic and helps attackers in gaining the access to a remote SQL server by exploiting the SQL injection vulnerability. It has a powerful AI system which easily recognizes the database server, injection type and best way to exploit the vulnerability” (Shankdhar, 2019).

SQL Injection Countermeasures
	One of the first countermeasure is to filter all input before it is entered into SQL queries. This should be applied to all types of input, including drop-down boxes and radio buttons, not only text boxes. However, this in itself is not enough to provide sufficient protection against more advanced SQL injection attacks because it does not solve the deeper problem. Therefore, there are many other mitigation strategies that web applications must implement.
	Patches and updates must be applied to all software packages, libraries, operating systems, plug-ins, web server software, and any other component used in the development of the web application. The principle of least privilege should be used when generating new user accounts, so more power is only granted to those who need it. If a web application only requires a SELECT statement, only grant it usage to SELECT statements and no other types of statements. Databases should not be shared between web applications (How to Protect Against SQL Injection Attacks).
	
Method: Cross-Site Scripting (XSS)

Like SQL injection, Cross-Site Scripting is also one of the most common types of web application attacks. “Hackers inject malicious scripts in trusted websites to harm both the website and its visitors” (Alexander). “Cross-site scripting ('XSS' or 'CSS') attacks exploit vulnerabilities in dynamically generated web pages, which enables malicious attackers to inject client-side script into web pages viewed by other users. It occurs when invalidated input data is included in dynamic content that is sent to a user's web browser for rendering. Attackers inject malicious JavaScript, VBScript, ActiveX, HTML, or Flash for execution on a victim's system by hiding it within legitimate requests. Attackers bypass client-ID security mechanisms and gain access privileges, and then inject malicious scripts into specific web pages. These malicious scripts can even rewrite HTML website content.” (Gregg & Santos, 2020)
	
Cross-Site Scripting  Tools
Find XSS - “If you seek a simple project-based tool that will help find cross-site scripting problems across a website or a PHP project, Find XSS is one of the most trusted tools that you’d find. Their website offers a detailed explanation of how to get started.”
XSS Mister Scanner - “tests your website for even the deep-seeded issues including the ones in your header, which seemingly look benign. Other that that, this scanner is capable of testing for every other server and OWASP issue including SQL Injection, Caching loopholes, and Cross-site Request Forgery.”
Quttera - “When it comes to detecting Cross-Site Scripting, Quttera is one of the best online testing tools in the market. Although it is not restricted to one vulnerability detection, you can use it the way you like it.”
XSS Scanner - “XSS Scanner is another free, basic tool that every developer should possess. You can test it out today and if it looks good, opt for the premium scans which also include periodic testing of the website. In the premium plan, you even get alerts for critical vulnerabilities found during the scan” (Alexander).

Cross-Site Scripting Countermeasures
	A few mitigations can defend against a very large numbers of XSS vectors. It is important to be careful in placing untrusted data from users. Data should be encoded before being inserted into the following locations on an HTML page: HTML element, HTML attribute, JavaScript data values, HTML style property values, and URL parameter values. However, it is always important to remember that “Developers SHOULD NOT put data into any other slots without a very careful analysis to ensure that what they are doing is safe. Browser parsing is extremely tricky and many innocuous looking characters can be significant in the right context.” (Cross Site Scripting Prevention Cheat Sheet)
	
Method: Command Injection
Command injection is another type of injection like SQL injection. It is also one of the most dangerous types of web application attacks. When attackers are able to bypass security of a web application to perform a command injection attack, they are able to run malicious commands to systems such as operating systems, shells, and calls databases. Web applications require operating systems, so they are close to the web applications under attack. “Command injection attacks are easy to carry out and discover, but they are difficult to understand.” (Gregg & Santos, 2020)
	
Command Injection Tools
Commix - “to test web applications with the view to find bugs, errors or vulnerabilities related to command injection attacks. By using this tool, it is very easy to find and exploit a command injection vulnerability in a certain vulnerable parameter or string. Commix is written in Python programming language” (Commix). Commix is a very popular command injection testing tool.

Command Injection Countermeasures
	“Carefully scrub an application before passing piece of information through an HTTP external request. Otherwise, attackers can insert special characters, malicious commands, and command modifiers into information.” (Gregg & Santos, 2020)
	
Method: Cross-Site Request Forgery
	“Cross-site request forgery (CSRF) is an attack which forces an end user to execute unwanted actions on a web application to which they are currently authenticated” (Using Burp to Test for Cross-Site Request Forgery (CSRF). It is not good for applications to rely only on HTTP cookies for knowing when the user has sent a request. CSRFs many times are achieved when an attacker sends a malicious link (that appears as a real link) that exploits the trust between the user and the client.
	
Cross-Site Request Forgery Tools
Burp Suit - Burp Suite Professional is one of the most popular penetration testing and vulnerability finder tools, and is often used for checking web application security (Huron, 2020). Burp scanner is able to quickly locate CSRF issues. Burp proxy is able to also help with CSRFs. 

Cross-Site Request Forgery Countermeasures
	Countermeasures include keeping anti-virus software updated, avoid opening untrustworthy emails, logging off applications, avoid saving passwords in browser, and disable scripting in browser. It is also good to “Check the HTTP Referrer header and when processing a POST, ignore URL parameters” (Gregg & Santos, 2020).
	
Conclusion

Testing for web application vulnerabilities is an important step in pen testing a network. Large companies will have many applications that will each require extensive testing to meet minimum requirements for deployment. There are many security firms that provide pen testing services, including ScienceSoft, Acunetix, Netsparker, CyberHunter, Raxis, and ImmuniWeb. (Top 10 Penetration Testing Companies and Service Providers (Rankings)). Sometimes, before someone can think like a cybersecurity professional, he/she must first think like a malicious attacker, which makes ethical hacking a valuable tool for securing networks.

References:

Alexander, G. 9 Cross-Site Scripting (XSS) Scan Testing Tools Online. MisterScanner. https://misterscanner.com/xss-testing-tool/. 

Commix. Penetration Testing Tools. https://tools.kali.org/exploitation-tools/commix. 

Cross Site Scripting Prevention Cheat Sheet. OWASP Cheat Sheet Series. https://cheatsheetseries.owasp.org/cheatsheets/Cross_Site_Scripting_Prevention_Cheat_Sheet.html. 

Gregg, M., & Santos, O. (2020). CEH: Certified ethical hacker version 10. Honoken, NJ: Pearson.

How to Protect Against SQL Injection Attacks. How to Protect Against SQL Injection Attacks | Information Security Office. https://security.berkeley.edu/education-awareness/best-practices-how-tos/system-application-security/how-protect-against-sql.

Huron, S. (2020, May 18). Burp Suite Professional for Web Application Security. Delta Risk. https://deltarisk.com/blog/how-to-use-burp-suite-professional-for-web-application-security-part-one/. 

Shankdhar, P. (2019, February 15). Best Free and Open Source SQL Injection Tools [Updated 2019]. https://resources.infosecinstitute.com/topic/best-free-and-open-source-sql-injection-tools/. 

Spencer, P. (2020, May 20). 43% of Data Breaches Connected to Application Vulnerabilities: Assessing the AppSec Implications. Security Boulevard. https://securityboulevard.com/2020/05/43-of-data-breaches-connected-to-application-vulnerabilities-assessing-the-appsec-implications/. 

Top 10 Penetration Testing Companies and Service Providers (Rankings). (2020, September 13). https://www.softwaretestinghelp.com/penetration-testing-company/. 

Using Burp to Test for Cross-Site Request Forgery (CSRF). PortSwigger. https://portswigger.net/support/using-burp-to-test-for-cross-site-request-forgery. 
