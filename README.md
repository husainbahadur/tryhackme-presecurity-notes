What was the objective?
What tools you used?
What you found?
What you learned?
# Module 1 - Introduction to Cyber Security
**Offensive Security**: where you simulate a hacker's actions to find vulnerabilities in a system?

**Terminal**: also known as the command line interface, is a program that allows user to send text-based commands to the computer.

**Defensive Security**: also known as blue team play a key role in protecting networks and organisations across the globe.

**SOC**: Security Operations Center is a team of IT security professionals tasked with monitoring, preventing , detecting , investigating, and responding to threats within a company’s network and systems.

**SIEM**: which is Security Information and Event Management and where systems are the central place for all data and information collected from security devices, workstations, servers, and more within an organisation.
## Offensive Security Intro
The objective was to hack a fake bank website and send 2000 to my account in a virtual machine. The overall goal was to show how an ethical hacker operates.

The tool I used was called dirb. This tool uses a brute-force approach, by taking a list of potential page names and testing one by one if they existed in the fake bank website.

I found that there were two hidden pages name and one had "BANK-DEPOSIT" at the end of the url which I copied and pasted into my Firefox browser and sent my account 2000. 

I learned that the core of Offensive Security is that "To outsmart a hacker, you need to think like one." as it involves...
- Breaking into Computer systems
- exploiting software bugs
- Finding loopholes in applications to gain unauthorised access

Overall, the goal of Offensive Security is to  understand hacker tactics and enhance company’s system defences before real hackers do.

I also learned that, A terminal (command line interface) is a program that allows users to send text-based commands to the computer. And lot of hacking tools, including dirb, need to be executed from a terminal. This is because the terminal is much more efficient then GUIs and Menus as it allows the user to directly talk to the software.
## Defensive Security Intro
The objective was to investigate a Web discovery attack on a fake bank website in a virtual machine, which is cool because I think it's the attack that I did at the start when learning about Offensive Security.

The tools I used, in the virtual machine was a Security Analyst Dashboard, where I could see all security event particularly a web discovery attack, upon further investigation I could see an Attack Summary which showed:
- Attacks started date
- Duration
and more like sorce IP, URLs attempted. The most interesting one was the Attack Parttern and it showed:
- Attack Type: Directory Enumeration
- Target: Admin Panels
- Method: Automated Scanning
- Risk Level: Medium

This makes sense as the method I used was dirb tool to scan for any hidden pages on the fake bank site and my target was the admin panel, and I think the directory enumeration means the hacker(me) used a directory like the Terminal. Also I responded to the attack by copying the source IP and blocking it form accessing the fake bank website basicall, I IP banned the hacker.

I found out that SOCs are the defensive security centres for organisation's technology. This centre is the frontline of protecting an organisation, often operating around 365 days a year, and employs a variety of security professionals who monitor and protect the organisation's networks, systems, and data.

A typical day in the Security Operation Cemtre looks like:
- Reviewing alerts triggered by security tooling
- Investigating anomalies
- Responding to incidents

overall, These professionals are basically the eyes and ears on the frontline for protecting an organisation.

I learned some key areas of defensive security:

- Monitoring and Detecting: Continually observing network and system activity to detect suspicious behaviour and events. These may include, for example, monitoring for logins from another country while the employee is based in the company's London office.

- Incident Response: The team quickly comes together if suspicious activity is confirmed and alerts are raised. This is when the Incident Response process begins.The process involves containing and removing the threat and restoring the business back to normality.
 
- Threat Intelligence: Gathering and using information about attackers trough their latest methods, targets, and trends—can greatly strengthen an organisation’s defences.For example, understanding that an attacker focuses on a specific software application used within organisations.

- Vulnerability Management: Fixing software or system flaws is an important preventative measure that can lower the risk of an attack. Security teams can check which systems attackers are most likely to target. This can be done manually or with the help of automated tools.

- Investigation and Analysis: Members of a defensive security team are always monitoring and analysing what’s happening inside an organisation.They work to separate normal activity from suspicious behaviour, digging into the details like solving a puzzle to uncover valuable insights.

I also learned that organisations don’t rely on a single tools and method to stay secure as they build layers of defences, this is called "Defence in Depth," meaning that if one security measure fails, the organisation have others to rely upon at various stages.

Examples of defensive measures include:
 
- Employee Training: In today's world, the human factor of cyber security cannot be ignored, because attacks more often than not targeting employees rather than systems this is called social engineering, training employees to be proactive in recognising attempts for things like phishing is essential.

- Intrusion Detection Systems (IDS):These devices act as surveillance cameras across the organisation's IT.They monitor and alert when suspicious behaviour or activity is detected across the network or systems.
 
- Firewalls: These devices act as security guards on an organisation's network.They monitor and determine what traffic is allowed to enter the network, or should be rejected.

- Security Policies: Security policies help organisations ensure that their systems are used correctly.They can reduce risk by blocking access to dangerous websites or requiring strong passwords, making it harder for attackers to guess login details.

## Careers in Cyber
I learned about 7 careers in Cyber Security, **Security Analyst** who are responsible for maintaining the security of an organisation's data, **Security Engineer** who design, monitor and maintain security controls, networks, and systems to help prevent cyberattacks, **Incident Responder** who jdentifies and mitigates attacks whilst an attackers operations are still unfolding, **Digital Forensics Examiner** are responsible for using digital forensics to investigate incidents and crimes, **Malware Analyst** who analyses all types of malware to learn more about how they work and what they do, **Penetration Tester** who are responsible for testing technology products for security loopholes and **Red Teamer** plays the role of an adversary, attacking an organisation and providing feedback from an enemies perspective.

Overview of all careers:

- **Security Analyst**:Security analysts are integral to constructing security measures across organisations to protect the company from attacks. Analysts explore and evaluate company networks to uncover actionable data and recommendations for engineers to develop preventative measures. This job role requires working with various stakeholders to gain an understanding of security requirements and the security landscape.

Responsibilities
Working with various stakeholders to analyse the cyber security throughout the company
Compile ongoing reports about the safety of networks, documenting security issues and measures taken in response
Develop security plans, incorporating research on new attack tools and trends, and measures needed across teams to maintain data security.
- **Security Engineer**:Security engineers develop and implement security solutions using threats and vulnerability data - often sourced from members of the security workforce. Security engineers work across circumventing a breadth of attacks, including web application attacks, network threats, and evolving trends and tactics. The ultimate goal is to retain and adopt security measures to mitigate the risk of attack and data loss.

Responsibilities
Testing and screening security measures across software
Monitor networks and reports to update systems and mitigate vulnerabilities
Identify and implement systems needed for optimal security
- **Incident Responder**:Incident responders respond productively and efficiently to security breaches. Responsibilities include creating plans, policies, and protocols for organisations to enact during and following incidents. This is often a highly pressurised position with assessments and responses required in real-time, as attacks are unfolding. Incident response metrics include MTTD, MTTA, and MTTR - the meantime to detect, acknowledge, and recover (from attacks.) The aim is to achieve a swift and effective response, retain financial standing and avoid negative breach implications. Ultimately, incident responders protect the company's data, reputation, and financial standing from cyber attacks.

Responsibilities
Developing and adopting a thorough, actionable incident response plan
Maintaining strong security best practices and supporting incident response measures
Post-incident reporting and preparation for future attacks, considering learnings and adaptations to take from incidents
- **Digital Forensics Examiner**:If you like to play detective, this might be the perfect job. If you are working as part of a law-enforcement department, you would be focused on collecting and analysing evidence to help solve crimes: charging the guilty and exonerating the innocent. On the other hand, if your work falls under defending a company's network, you will be using your forensic skills to analyse incidents, such as policy violations.

Responsibilities
Collect digital evidence while observing legal procedures
Analyse digital evidence to find answers related to the case
Document your findings and report on the case
- **Malware Analyst**:A malware analyst's work involves analysing suspicious programs, discovering what they do and writing reports about their findings. A malware analyst is sometimes called a reverse-engineer as their core task revolves around converting compiled programs from machine language to readable code, usually in a low-level language. This work requires the malware analyst to have a strong programming background, especially in low-level languages such as assembly language and C language. The ultimate goal is to learn about all the activities that a malicious program carries out, find out how to detect it and report it.

Responsibilities
Carry out static analysis of malicious programs, which entails reverse-engineering
Conduct dynamic analysis of malware samples by observing their activities in a controlled environment
Document and report all the findings
- **Penetration Tester**:A penetration tester's job role is to test the security of the systems and software within a company - this is achieved through attempts to uncover flaws and vulnerabilities through systemised hacking. Penetration testers exploit these vulnerabilities to evaluate the risk in each instance. The company can then take these insights to rectify issues to prevent a real-world cyberattack.

Responsibilities
Conduct tests on computer systems, networks, and web-based applications
Perform security assessments, audits, and analyse policies
Evaluate and report on insights, recommending actions for attack prevention
- **Red Teamer**:Red teamers share similarities to penetration testers, with a more targeted job role. Penetration testers look to uncover many vulnerabilities across systems to keep cyber-defence in good standing, whilst red teamers are enacted to test the company's detection and response capabilities. This job role requires imitating cyber criminals' actions, emulating malicious attacks, retaining access, and avoiding detection. Red team assessments can run for up to a month, typically by a team external to the company. They are often best suited to organisations with mature security programs in place.

Responsibilities
Emulate the role of a threat actor to uncover exploitable vulnerabilities, maintain access and avoid detection
Assess organisations' security controls, threat intelligence, and incident response procedures
Evaluate and report on insights, with actionable data for companies to avoid real-world instances
# Module 2 - Network Fundamentals

## What is Networking?

## Intro to LAN

## OSI Model

## Packets & Frames

## Extending Your Network

# Module 3 - How The Web Works

## DNS in Detail

## HTTP in Detail

## How Websites Work

## Putting it all together

# Module 4 - Computer Fundamentals

## Inside a Computer System

## Computer Types

## Client-Server Basics

## Virtualisation Basics

## Cloud Computing Fundamentals

# Module 5 - Operating System Basics

## Operating Systems: Introduction

## Windows Basics

## Linux CLI Basics

## Windows CLI Basics

## Operating System Security

# Module 6 - Software Basics

## Data Representation

## Data Encoding

## Python: Simple Demo

## JavaScript: Simple Demo

## Database SQL Basics

# Module 7 - Attacks and Defenses

## The CIA Triad

## Cryptography Concepts

## Become a Hacker

## Become a Defender
