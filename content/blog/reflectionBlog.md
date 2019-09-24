---
title: "Week 2 Deliverable: Reflection"
date: 2019-02-17
pubtype: "Blog"
featured: true 
description: "This talk looked at Liberty Mutual’s transformation to Continuous Integration, Continuous Delivery, and DevOps. For a large, heavily regulated industry, this task can not only be daunting, but viewed by many as impossible."
tags: ["xss","Bug Bounty","HackerOne","CI/CD pipelines","agile","Culture"]
image: "/img/Capturesom.PNG"
link: "http://www.kotaku.co.uk/2018/11/13/valve-pays-15000-to-hacker-who-found-steam-bug-that-generates-free-games"
fact: "Interesting little tidbit shown below image on summary and detail page"
weight: 400
sitemap:
  priority : 0.8
---

<h3>Introduction</h3>

Week 2 has been a very interesting week where I went deeper into cyber security knowledge base. It had been a great experience with the subject so far, I had been involved in fixing my website, working on challenges on PentesterLab, Juice-shop, Hackthebox.eu, writing and researching blogs such as hackerOne, BugsCrowd and working out the real life issues with the security in a company's online network and the various ways it can be exploited. This week I also learnt to manage my time between classes, work and homework as I was actively involved in everything that made me miss-out on some key points at my classwork activities that I had to do. I will be explaining more about these in this reflection.

On Monday I was involved in working on researching BugCrowd and HackerOne to write, How ethical hacking and bug bounties are impacting stakeholders and How you can implement things you've learnt throughout the week to test web apps under a responsible disclosure program. Which I have described it in here - <a href="vishaluniyal.gitlab.io/blog/week1blog/">Ethical Hacking Blog</a>. I have got the responsible disclosure concept of disclosing information such as bugs or vulnerabilities of the company by reporting to the company first before taking anyother actions. I haven't have much of experience in vulnerability exploiting that I can go ahead to find vulnerabilities for a company and report them, but in future I will become capable and I will surely keep in mind some of the main points I have gathered for responsible disclosure of any vulnerablities of any site <b>(SLO 1)</b> -

<ul>
    <li>Respect the privacy and not destroy people’s data. NEVER impact other users with your testing.</li>
    <li>Not to disclose the bugs to public unless a mutual agreement is made with the security team of that company.</li>
    <li>I will document the report in detail of how I exploited the bug so that it will be easier for the company to analyse and fix the bug.</li>
    <li>Respect other Bug hunters and respect company policies on any platform you are bug hunting and reporting.</li>
    <li>Take company’s consent before trying hacking their network or website.</li>
    <li>Always go through their, privacy and Terms and Conditions before performing any actions on live company network.</li>
</ul>

<h3>Portfolio Website Issues</h3> 

<p><b>SLO 4</b></p>nthlyufjglf

At week 1 I was able to create a website to write my blogs on gitlab but the website was a static website with no generator and basically hardcoded, which takes all the functionalities of basic generator website. Larry and Darsh told me that I will have to recreate my website with a generator in it. On Wednesday I sat down with Andy Lee to search options that we can use to create a generator website. We decided to use Jekyll to run our website, we were warned by other students that it will be a very challenging and we will be needing the right tools to get it working. But me and Andy took the challenge and sat down after class to install that framework. The other students like Jacob Ko, Frank Peng and Max were right about it. It became really hard and annoying, when we were just at the end of running the local server at our computer but the Jekyll framework kept on failing. We Finally decided to use Hugo, I still wanted to run Jekyll but I started installing Hugo and help Andy get his website up and running first. 

<p><b>SLO 3</b></p>
After successful installation of local server on Andy's machine (SLO 3) I had to prepare for my capstone project for the next day so I called it a day and went home. Frank Helped Andy to get the his protfolio website Live using Github. It was very generous of Andy to send me steps to publish my hugo website online. For some reason my website was still not publishing so the next day on Friday I asked Frank whether he can help me publish it. He was a great help as he setup my repository on gitlab and showed excatly what was going wrong in my steps. He pointed the address and the pipline I am using incorrect which was leading to failiure. If I hadn't known Frank and collaborated with other people I would have stuck with fixing Jekyll. (SLO 4)

<img src="/img/pipelineError.PNG" height="400px" width="800px"></img>
<p>Artifact 1: Errors Before my setup</p>
<br>
<img src="/img/PipeSuc.PNG" height="400px" width="800px"></img>
<p>Artifact 2: Successful running after collaborting with Frank and Andy</p>

<p><b>SLO 4 ^</b></p>

<h3>Solving Capture The Flag (CTF) Challenges</h3>

I have been solving Pentester Labs Examples,solving some of various methods a I can use XSS scripts and SQL injection to Hack into the and Exploit data. The example website gives you hint but not full solution which makes me logical reason how to go about exploit information and solving the basic myths of 1=1' if the that works. 

<img src="/img/pen1.PNG" height="200px" width="800px"></img>
<p>Artifact 3: XSS Exploit using "Image" tag</p>

<img src="/img/pen2.PNG" height="200px" width="800px"></img>
<p>Artifact 4: SQL Injection code to generate the next ID</p>

<p><b>SLO 2 </b></p>
<h3>Cracking Hackbox Website Invite code</h3>
<br>

When I heard of the website I searched it up and It had a invite code, I was sceptical that people will provide me a invite code. The website being for hackers, I guess I would have to "Invite Myself". I opened the Inspect element and spammed the submit button and I got a code, which I decrypted asked me to do a Post to a address. So I looked up google to how to do a post on PowerShell, and I did post with the given code bellow.

<code>curl -v -H "Content-Type: application/json" -X POST \
     -d '{}' https://www.hackthebox.eu/invite/api</code>
     <br>
From this I was able to get the actual invite code and I was able to get the invite code decrypted and I was able to login. This feeling was one of the greatest achievement for me, I felt like an actual hacker, I felt good and I wanted to do more of CTF challenges but before I practise on PentesterLab it gave me more logical questioning power that pushed me to unexpected solutions and results which were sucessful.
<br>

<br>
<img src="/img/hackbox1.PNG" height="400px" width="800px"></img>
<p>Artifact 5: InviteCode Hacking</p>
<br>
<img src="/img/hackbox2.PNG" height="400px" width="800px"></img>
<p>Artifact 6: Cracked code Using Powershell Curl</p>
<br>
<img src="/img/hackbox3.PNG" height="400px" width="800px"></img>
<p>Artifact 6: Finding the code Through decrypting</p>
<br>
<p><b>SLO 2 & 3 ^</b></p>

<br>
<h3>Reflection from Feedback and Research</h3>
<br>
<p><b>SLO 5</b></p>

Larry, Darsh and Luke have been really great help in providing me and the class feedback, providing resources to become a better at cyber Security, they are always engaging, friendly and polite with everyone. They are very sincere tutors and helpful especially when I had many work, interview related engagement this week. They gave me time to catch up with my work. From the previous week feedback I have to stick to my topic while I have giving my presentation, ask as many questions to understand my course and homework better. Be more engaging and collaborative in the class. 

However this week I tried my best to catch up with the class but I still haven't met the key reflective points just yet. Now I know where I should have a look at the Microsoft teams often to get more Information on what I should be contributing and should work toward the assignment before coming to the class. I will be able to manage my time better to be more collabortive in my class and Acheive better in my tutorials. Being collaborative helping others, people like Frank, Andy and Jacob giving me insights on my work and putting up a helping hand motivates me to work more towards cyber security and cracking CTF challenges to increase my knowlegde and Logical reasoning.

<p><b>SLO 5 ^</b></p>

<br>

<h3>References</h3>
<br>
<p class="">
                HackerOne, "Disclosure Guidelines". Accessed on 15-02-2019 - https://www.hackerone.com/disclosure-guidelines </p>
            <p class="">    Bug Crowd, "What is Responsible Disclosure?". Accessed on 15-02-2019 - https://www.bugcrowd.com/resource/what-is-responsible-disclosure/
        </p>

<p>Kalman. G, 2018, "10 Most Common Web Security Vulnerabilities". Accessed on 15-02-2019 - https://www.toptal.com/security/10-most-common-web-security-vulnerabilities</p>

<p>Vera Code, "SOFTWARE DEVELOPMENT LIFECYCLE (SDLC)
What is a Software Development Lifecycle?". Accessed on 15-02-2019 - https://www.veracode.com/security/software-development-lifecycle</p>
<p>PentesterLab, "Web for Pentester". Accessed on 15-02-2019 - https://pentesterlab.com/exercises/web_for_pentester/course</p>