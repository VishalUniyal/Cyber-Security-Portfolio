---
title: "Week 4 : SUMMER STUDIOS CYBER SECURITY: AN OFFENSIVE MINDSET REPORT"
date: 2019-02-27
pubtype: "Blog"
featured: true 
description: "This talk looked at Liberty Mutual’s transformation to Continuous Integration, Continuous Delivery, and DevOps. For a large, heavily regulated industry, this task can not only be daunting, but viewed by many as impossible."
tags: ["xss","Bug Bounty","HackerOne","CI/CD pipelines","agile","Culture"]
image: "/img/MicrosoftTeams-image(1).png"
link: "http://www.kotaku.co.uk/2018/11/13/valve-pays-15000-to-hacker-who-found-steam-bug-that-generates-free-games"
fact: "Interesting little tidbit shown below image on summary and detail page"
weight: 400
sitemap:
  priority : 0.8
---

Summer Studios has been great journey for me, I have came across many Cybersecurity tools, Get to meet professionals and get to know what is like to work in cybersecurity field from various big company's like delloit, Gitlab. I we got a chance to break into the Machines that these professionals provided,  


<h3>Objective</h3>
The reason I took up summer studio was I wanted to enrol in a cyber security subject where I can get to learn hacking, making software more secure, learn current popular tools in cyber security tools. 
From the Cyber Security Summer Studios Classes I wish to:
<br>
<ul>
<li> Develop me technical knowledge and Analytical skills on Cyber Security Issues</li>
<li> Collaborate with my team and gain knowledge from experienced veterans of Cyber Security fields</li>
<li> Reflect of my skills and improve on them from over time.</li>

<br>
<h3>Tools</h3>

<p><b>Environment – </b>Kali Linux, Windows 10 and various Virtual Machines</p>
<p>Programs – Metasploit, Aircrack-ng, Binaryninja, Hackthebox Virtual Machines.</p>
<br>
<h3>Intelligence Gathering</h3>

<p><b>Nmap –</b> is open source network scanning software for detecting devices connected in a network. It uses Raw IP packets to what hosts are available on network and what kind of services are provided by these hosts and what OS they are running. </p>

<p>
Nmap is Flexible which is, it can map multiple IPs, firewalls, routers, switch and other devices in the network. It is powerful as it can scan a huge network and is able to map thousands of machines on the network. Portable as it has support for all the main OS in the market.
The artefact bellow shows me using nmap to find version, Open ports to find loopholes into the system.
</p>

<img src="/img/backdoor.PNG" height="400px" width="800px"></img>
<p>Artefact 1 : Scanning through the network to get details of a specific IP.</p>

<br>
<p>
Net discover – Is a network discovering tool for discovering hosts on a wireless/wired networks, it sends ARP request and sniffs for reply. It is very easy to use, it is fast and a powerful tool to find any device connected to the network.
</p>

<img src="/img/final.PNG" height="400px" width="800px"></img>
<p>Artefact 2 : using ARP request to do network scan</p>
<br>
<h3>
Vulnerability Scanning
</h3>
 Msfconsole scanners – security networking tool used to exploit and penetrate systems for testing. It is the most popular tool amongst security researchers. This tool gives a great vulnerability test of a network and webapps.
WMAP - I used it in my web app exploitation in Metasploit. 
<br>
<img src="/img/some.PNG" height="400px" width="800px"></img>
<p>Artefact 3 : Testing target site to find vulnerabilities that can be exploited in a website.</p>

WP scan (WordPress Scanner)- Is an open source WordPress vulnerability scanner, many securities professional use these tools to test and maintain the security of their site. I have used WP scanner to scan into a WordPress website, with this I was able to get admin access to a WordPress website.
<br>
<img src="/img/wp2.PNG" height="400px" width="800px"></img>
<p>Artefact 4: Scanning a website URL to find vulnerabilities. (Mr. Robot CTF challenge)</p>
<br>
<img src="/img/wp7.PNG" height="400px" width="800px"></img>
<p>Artefact 5: Brute forcing into the website using Fireforce tool after finding vulnerability using WP Scan</p>
<br>

<img src="/img/wp8.PNG" height="400px" width="800px"></img>
<p>Artefact 6: Gained Access into the Word Press Website. </p>

<br>

<h3>Exploitation</h3>
<br>
<b>Getting Root Access – </b> Gaining root access to a website or machine gives the hacker/pen tester the high privileges to a that device and hacker can exploit is other resources very easily. Happens when a device doesn’t have the latest software update and it can be exploited. You can view my past work of getting root access in my portfolio website blog here - https://vishaluniyal.gitlab.io/blog/week3blog/
Metasploit is the easiest way to exploit a machine, you can run vulnerability scans and then set the target machine that you want to exploit.
<br>
<img src="/img/Captureexploit.PNG" height="400px" width="800px"></img>
<p>Artefact 7: Setting target Host Machine and Exploiting it using Metasploit</p>
<br>
<img src="/img/rootshell.PNG" height="400px" width="800px"></img>
<p>Artefact 8: Gained Root access to a machine</p>
<br>
<img src="/img/maround.PNG" height="400px" width="800px"></img>
<p>Artefact 9: Exploiting a User account on the machine</p>
<br>
During my session I learnt BinaryNinja tool to view and crack binary files to break through encryption and reveal the hidden message. I used this tool to complete “Evil Morty challenge” To get the message inside a binary encoded file.
<br>
<img src="/img/flag.PNG" height="400px" width="800px"></img>
<p>Artefact 10: Using Binary Ninja tool to get the hidden message.</p>
<br>

<h3>Executive report</h3>
<br>
Pen testing, Cyber Security, Intelligence Gathering has a very high impact to a Industry which relies on IT or web application for business. I have mention my summary about the potential business impact on my blog here - https://vishaluniyal.gitlab.io/blog/week1blog/
<br>
Company can lose its reputation when it gets exploited and the data is leaked to the public, The stakeholder lose faith in the company’s data security and start finding alternatives. It is a high value market loss and a breach to user’s confidential information. Users can sue the company for not having kept their data safe and company will incur huge financial losses.
Solution to this problem is continuously testing the software environment e.g. Unit Testing, to check the other parts of program doesn’t fail whenever a new feature is introduced. Register your company with bug bounty program like HackerOne or BugsCrowd so that ethical hackers find vulnerabilities for the company and get rewarded.
<br>

<h3>Presentations</h3>
<h5>SLO4</h5>
Throughout this course we have been involved in weekly presentations on our research on various topics. My first presentation was on Bug Bounties – many people in our class are unaware of bug bounties, which is a way of testing vulnerability and exploits of an IT or Fintech company and get paid lump sum if the exploit will has a very severe impact on a company.

<img src="/img/MicrosoftTeams-image(1).png" height="400px" width="800px"></img>
<p>Artefact 11:  Group Presentation on Bug Bounties (Week 1)</p>
<br>
It was a very fun experience working and research with my team,  I got learn and research about interesting topic one being bug bounty and the other on AirCrack-ng.
Presentation on Aircrack – Firstly about Aircrack, it is a opensource Wifi cracking tool which come in a suite where you can find AirDump (gets all wifi packets), Airmon and more. I got the basics of how to use these tool while researching in my presentation and get to present and share my knowledge with everyone who haven’t used AirCrack before.
<br>

<h3>Conclusion</h3>
<h4>SLO5</h4>
<br>
The tutors are really helpful, they put all the useful cyber security related material on the group chat, and give us feed back after every sprint session for us to reflect and improve on. My experience with this subject is very energetic, enjoyable and hear about the future activities from Larry and Darsh I am really excited to be part of Cyber Security Summer Studios. So far my performance according to Darsh and Larry are above average but to become more better at this field I will have to crack more challenges in Hack the Box and many other popular challenges to become more competative in this industry.
<br>

<h3>References</h3>
<p>WordPress Scanner, Accessed on 05-03-2019 - https://wpscan.org/</p>
<p>Infosec Institute, Vulnerability scanning metapoilt part 2, Accessed on 05-03-2019 https://resources.infosecinstitute.com/vulnerability-scanning-metasploit-part-2/#gref
</p>
<p>
https://www.offensive-security.com/metasploit-unleashed/wmap-web-scanner/
</p>
<p>
Network Map, General Blog, Accessed on 05-03-2019 - https://nmap.org/
</p>
<p>
Vishal Uniyal, Blog- Accessed on 05-03-2019 - https://vishaluniyal.gitlab.io/
</p>




