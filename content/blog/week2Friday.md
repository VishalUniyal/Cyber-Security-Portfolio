---
title: "Week 2 HomeWork 2 : Problem Statement on Web-application Security"
date: 2019-02-15
pubtype: "Blog"
featured: true 
description: "This talk looked at Liberty Mutual’s transformation to Continuous Integration, Continuous Delivery, and DevOps. For a large, heavily regulated industry, this task can not only be daunting, but viewed by many as impossible."
tags: ["xss","Bug Bounty","HackerOne","CI/CD pipelines","agile","Culture"]
image: "/img/npm.PNG"
link: "http://www.kotaku.co.uk/2018/11/13/valve-pays-15000-to-hacker-who-found-steam-bug-that-generates-free-games"
fact: "Interesting little tidbit shown below image on summary and detail page"
weight: 400
sitemap:
  priority : 0.8
---



<h2>OWASP XSS</h2>
<h3>Introduction</h3>
Web applications are susceptible to attacks that may result in exposure or modification of sensitive data, or impact on availability of services to authorized users.  Application testing is conducted to identify security flaws introduced in the design, implementation or deployment of an application.  Developers and application administrators must identify functions that are critical to security and test those functions to verify correct operation.

<h3>Problem Statement #1 - Cross Site Scripting (XSS)</h3>

Cross Site Scripting (XSS) is a fairly widespread input sanitization failure (essentially a special case of common mistake #1). An attacker gives your web application JavaScript tags on input. When this input is returned to the user unsensitized, the user’s browser will execute it. It can be as simple as crafting a link and persuading a user to click it, or it can be something much more sinister. On page load the script runs and, for example, can be used to post your cookies to the attacker.
Prevention: There’s a simple web security solution: don’t return HTML tags to the client. This has the added benefit of defending against HTML injection, a similar attack whereby the attacker injects plain HTML content (such as images or loud invisible flash players) – not high-impact but surely annoying. Usually, the workaround is simply converting all HTML entities, so that <code>script</code> is returned as <code>&ltscript&gt</code>. The other often employed method of sanitization is using regular expressions to strip away HTML tags using regular expressions on < and >, but this is dangerous as a lot of browsers will interpret severely broken HTML just fine. Better to convert all characters to their escaped counterparts.

<h3>Problem Statement #2 – SQL Injection</h3>
Injection flaws result from a classic failure to filter untrusted input. It can happen when you pass unfiltered data to the SQL server (SQL injection), to the browser (XSS) to the LDAP server (LDAP injection), or anywhere else. The problem here is that the attacker can inject commands to these entities, resulting in loss of data and hijacking clients’ browsers. Anything that your application receives from untrusted sources must be filtered.

Prevention: protecting against injection is “simply” a matter of filtering your input properly and thinking about whether an input can be trusted. But the bad news is that all input needs to be properly filtered, unless it can unquestionably be trusted.

Review the OWASP guidelines.  Identify those potential vulnerabilities that may apply to your web application. Review your code and test your application to ensure that your application is not vulnerable.  (See the Related Procedures and Resources section below for the link to more detailed information about these software vulnerabilities.)

 
Using XSS and SQL injects examples to practise ways of injection can be performed on a fairly vulnerable website.

 
XSS is very easy to exploit in Juice-shop CTF website.
I was able to get admin access to the website and was able to change terms and conditions that were given on the Juice-shop website. It also gave me a list of all user credentials via SQL Injection. This shows website is returning a HTML tags to The client and it is not sanitising the script expression and also not SQL scripts. If the apply the above prevention system, it will really hard to crack it next time.
<br>

<h3>Related Procedures and Resources:<h3>
<h4>Campus Standards and Practices</h4>
<ul>
<li><a href="https://security.calpoly.edu/content/exception-process">IT / Information Security Exception Request Process</a></li>
<li><a href="https://security.calpoly.edu/content/vulnerability">Vulnerability Assessment and Management Standard</a></li>
<li><a href="https://security.calpoly.edu/content/policies/asset-risk-definition">Information Asset Risk Level Definition</a></li>
</ul>


<h3>How do these issues effect a business? </h3>

Today's increasingly complex software development environment requires elegant and comprehensive solutions. Developers must juggle numerous tools and technologies while producing code that performs at the level of digital business. Teams must address an array of issues, including coding to APIs, mobile, and cloud environments. Too many tools lack the flexibility required for developers and many also come with a steep learning curve.
 
It's essential to adopt tools that detect application security vulnerabilities and integrate risk data and metrics in an automated fashion. Organizations that introduce an integrated approach to security and build protection into their SDLC can reduce risk, trim costs, and speed development. They’re able to develop new applications and continuously update existing software without sacrificing security.
 
<h3>More Solutions : Embedding Security Testing into Your SDLC<h3>

<h4>Unit Testing</h4>

All security-sensitive code should have a corresponding test suite which verifies that every outcome of every security decision works properly. It greatly improves the odds of catching vulnerabilities before they emerge as actual breaches.
Black Box Testing

It is a critical component for application security — and it’s an integral part of a SDLC framework. The black box analysis searches inside debug code, directories, leftover source code, and resource files to find SQL strings, ODBC connectors, hidden passwords or usernames, and other sensitive information that malicious individuals could use to hack an application.
White Box Testing

The ability to find and fix coding vulnerabilities promptly is nothing less than critical. Veracode's white box test solution uses static analysis to spot common flaws without actually executing the software.
As the digital age matures and as software code becomes part of every product, service, and business process, it's clear that there's a strong need for a comprehensive and holistic approach to application security. A business and security framework that revolves around a software development lifecycle is all about dollars and sense.

<h3>REFERENCES</h3>
https://security.calpoly.edu/content/standards/web-app-vulnerabilities?fbclid=IwAR18jbTchzMceIOjAe4R2JKCwF4ajl3RREdxGJdoeE_-XRnMkrUDuYTG7Bs

https://www.toptal.com/security/10-most-common-web-security-vulnerabilities?fbclid=IwAR2hT8UREHqvjUrfKRsOV_02Bz1xZI3LzuH-XEX3PQpSx05-s9aSiVWYimE

https://www.veracode.com/security/software-development-lifecycle?fbclid=IwAR2U0vMWPSX4KHPdw05LGT90p-JHXwPXFgpfrxDleXFnzoOm7fPrpCdOFo8






 