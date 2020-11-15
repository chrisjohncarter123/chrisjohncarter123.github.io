---
layout: post
title:      "SQLSniper Tool Project"
date:       2020-11-15 03:08:00 +0000
permalink:  sqlsniper_tool_project
---


I have been studying cybersecurity and ethical hacking recently, and I have learned many types of networking attacks. SQL injection is one of the most dangerous and common attack. According to [OWASP](https://owasp.org/www-project-top-ten/), injection is the number one web application security risk. Therefore, I thought it would be enjoyable to write a tool that performs automated SQL injection on a target website to test for vulnerabilities. I plan on writing the application in Ruby, and will use the command line for an interface.

The first step I would like to complete in development is implementing functionality to perform the simplest possible SQL injection attack. Here are the steps it would perform:

1. The user would enter their input into the command line. For example, a website URL with a form with a input field and a submit button
2. The user will enter the desired function to execute on the target's database.
3. SQLSniper will automatically generate the correct string to enter the form and submit it. It will then return the response from the server.

This the absolute minimum functionality needed for the tool to be useful. I would like to further develop functionality that provides firewall evading, information gathering, database column gathering, and advanced automation. My end goal is for a user to provide a base URL, and the tool will automatically scan as many forms as possible for SQL injection. It may run hundreds of SQL statements on a single form, which would be very tedious to do without automation. There are also many different types of SQL injection, and it would be nice to implement some of them such as error-based, incorrect query, and piggybacked query.

There are many variations to performing SQL injection attacks. There are also many techniques that bypass firewalls, IDS, and other types of networking security. I am amazed at how fast new vulnerabilities are being discovered. Hopefully this tool will be useful in pen testing and ethical hacking. It may be impossible to keep up with all of the new trends and tricks discovered.

Sources:

https://owasp.org/www-project-top-ten/
