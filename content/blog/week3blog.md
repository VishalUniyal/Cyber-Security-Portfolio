---
title: "Week 3 Reflection: Problem Statement on Web-application Security"
date: 2019-02-24
pubtype: "Blog"
featured: true 
description: "This talk looked at Liberty Mutual’s transformation to Continuous Integration, Continuous Delivery, and DevOps. For a large, heavily regulated industry, this task can not only be daunting, but viewed by many as impossible."
tags: ["xss","Bug Bounty","HackerOne","CI/CD pipelines","agile","Culture"]
image: "/img/npm.PNG"
link: 
fact: "Interesting little tidbit shown below image on summary and detail page"
weight: 400
sitemap:
  priority : 0.8
---

Week 3 was a great sprint where I got a chance to meet cyber security people from delloit, I got to hack to get administrator access to both a machine and a Wordpress website. I learnt alot on how the cyber security industry works. 

On monday I learnt the Vm and the Wordpress CTF challenges that I have to do to get through the sprint and I started working on that, Where I was able to gain root access to the ubuntu Virtual Machine and the password. We also had to prepare for a group presentation for Wednesday. I decided what we are going to present on which was AIRCRACK-ng where I took the initiative of doing the main topic on explaining about aircrack (Slide 5 and 6) and showing it in action. You can view our presentation at - https://docs.google.com/presentation/d/1mH4f4ga8g755NWiLRoq_wTtxcDtnLqWot66_N0-ESzY/edit

<img src="/img/2.PNG" height="400px" width="600px"/>
<br></br>
Artifact 1: Discovering Victim VMs IP address
<br></br> 
<img src="/img/backdoor.PNG" height="400px" width="600px"/>
<br></br>
Artifact 2: Gaining Backdoor access 
<br></br>
<img src="/img/exploring passs.PNG" height="400px" width="600px"/>
<br></br>
Artifact 3: Exploring passwords using wordlist dictionary to get credentials
<br></br>
<img src="/img/found pass.PNG" height="400px" width="600px"/>
<br></br>
Artifact 4: Found Passwords
<br></br>
<img src="/img/Captureexploit.PNG" height="400px" width="600px"/>
<br></br>
Artifact 5: Changing Target Address to Victim VM and Initiating Exploit
<br></br>
<img src="/img/root shell.PNG" height="400px" width="600px"/>
<br></br>
Artifact 6: Gained root access
<br></br>
<img src="/img/messing around.PNG" height="400px" width="600px"/>
<br></br>
Artifact 7: Exploiring Victims VM and finding more exploits.
<br></br>

<h5>SLO 4</h5>
It was a bit hard to follow these steps when I am doing on my own, I took help from classmates like Andy Lee and Frank Peng and spread this knowledge to other student who were struggling to gain Admin access to the Basic Pentesting 1 Virtual Machine. I took some help by looking at the youtube videos for reference -  https://www.youtube.com/watch?v=Ls3bwlaiSX8&index=2&list=PLg898sqAkgc8VobP2xl8d_zqIESvltA-f

<h5>SLO 1</h5>
On Wednesday I prepared a script for what I am going to say in my presentation and organised our presentation slides and made it more presentable. On the first half we had a cybersecurity officals from delloite comming in. They gave a good insight about their company and how flexible the cybersecruity division is in thier company. They allowed us to use their VM to hack into it. I followed the steps they told us to get into their machines and I was able to get user access to their virtual machine they provided. I learnt how their strategy of breaking into their VM was. They gave out hints that helped us to think more logical towards cracking their passwords. (SLO 1)

<h5>SLO 2</h5>
On Friday I continued my hacking a Mr Robot Wordpress website as per deliverable requirement. I was able to get Root Shell access, thanks to Andy Lee he gave me a basic Idea of how this work and why we require a VPN to access such sites. I took notes on Darsh's step by step demonstration to hack into a wordpress website. It helped me alot to understand how the wordpress firmware works. I was a bit hard to gain access to yhe wordpress site, so I referred to multiple videos on youTube and approached other students like Andy, Max and Ian to get a best ways to extract Keys and break into the website. I found a way to get to the website but I am still unclear how to get the remaining hidden CTF keys to crack Wordpress, I will try to practice and get those keys next week in week 4.(SLO 2)

<br></br>
<img src="/img/wp1.PNG" height="400px" width="600px"/>
<br></br>
Artifact 8: Getting access to the ports of the Wp mr robot website
<br></br>
<img src="/img/wp2.PNG" height="400px" width="600px"/>
<br></br>
Artifact 9: Scanning the WP URL for Vulnerabilities or lose URL or text files (Found robot.txt)
<br></br>
<img src="/img/wp3.PNG" height="400px" width="600px"/>
<br></br>
Artifact 10: Discovering txt files and loose plugins
<br></br>
<img src="/img/wp5.PNG" height="400px" width="600px"/>
<br></br>
Artifact 11: Found 1st key
<br></br>
<img src="/img/wp6.PNG" height="400px" width="600px"/>
<br></br>
Artifact 12: Using Sparta to find Vulnerabilites
<br></br>
<img src="/img/wp7.PNG" height="400px" width="600px"/>
<br></br>
Artifact 13: Username found and using Fireforce plugin to bruteforce into website
<br></br>
<img src="/img/wp8.PNG" height="400px" width="600px"/>
<br></br>
Artifact 14: Got access to the Dashboard.
<br></br>

<h5>SLO 3</h5>
I did multiple free for alls this week and got to know John Wey, Andy Lee, Ian problems they are facing. They were a step ahead in where I currently solved but they all had different approaches to the problem. Ian had a tool called fireforce on kali firefox that uses somesort of bruteforce to crack the password. Andy showed me a glimpse of Sparta to show how he can detect multiple vulnerabilities and enumerate it. I used these techniques to crack my Wordpress admin.(SLO 3)

<h5>SLO 5</h5>
There are still alot of tools and strategies I need to learn to break into a website. By interacting with other experienced students I got to know tools that I never heard of before like Sparta, FireForce and zenmap, that I can use to make my breaking process more simpler and faster. I am quickly developing the mind of an hacker and a Cybersecurity official and applying strategies that are unsual and never used before. Feedback from tutors are very helpful these artifact help me to reflect my progress and push me to do better. Also helps me to refer to it to give me a different approach to crack a problem. I will carefully note down all the steps which Darsh uses during his demonstration which are really valuable simple and are the ideal way to do it. (SLO 5)

<h3>References</h3>

Basic Penetration Testing 1 - walkthrough, Accessed on 20/02/2019 https://www.youtube.com/watch?v=Ls3bwlaiSX8&index=2&list=PLg898sqAkgc8VobP2xl8d_zqIESvltA-f

Mr Robort CTF, Try Hack Me. Accessed on 23/02/2019 - https://tryhackme.com/room/mrrobot

Mr. Robot CTF Hacking Walkthrough, Accessed on 23/02/2019 - https://www.youtube.com/watch?v=0VJyfJzbPE4