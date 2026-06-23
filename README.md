I completed this course on the free tier of TryHackMe. Where I hit a paywall, I've documented what I was able to cover in each module. Even when I couldn't go further inside the platform, I looked into the topics independently because I was genuinely curious.
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

- **Security Analyst**: are integral to constructing security measures across organisations to protect the company from attacks. Analysts explore and evaluate company networks to uncover actionable data and recommendations for engineers to develop preventative measures. This job role requires working with various stakeholders to gain an understanding of security requirements and the security landscape.

**Responsibilities**:
- Working with various stakeholders to analyse the cyber security throughout the company
- Compile ongoing reports about the safety of networks, documenting security issues and measures taken in response
- Develop security plans, incorporating research on new attack tools and trends, and measures needed across teams to maintain data security.

- **Security Engineer**: develop and implement security solutions using threats and vulnerability data - often sourced from members of the security workforce. Security engineers work across circumventing a breadth of attacks, including web application attacks, network threats, and evolving trends and tactics. The ultimate goal is to retain and adopt security measures to mitigate the risk of attack and data loss.

**Responsibilities**:
- Testing and screening security measures across software
- Monitor networks and reports to update systems and mitigate vulnerabilities
- Identify and implement systems needed for optimal security

- **Incident Responder**: respond productively and efficiently to security breaches. Responsibilities include creating plans, policies, and protocols for organisations to enact during and following incidents. This is often a highly pressurised position with assessments and responses required in real-time, as attacks are unfolding. Incident response metrics include MTTD, MTTA, and MTTR - the meantime to detect, acknowledge, and recover (from attacks.) The aim is to achieve a swift and effective response, retain financial standing and avoid negative breach implications. Ultimately, incident responders protect the company's data, reputation, and financial standing from cyber attacks.

**Responsibilities**:
- Developing and adopting a thorough, actionable incident response plan
- Maintaining strong security best practices and supporting incident response measures
- Post-incident reporting and preparation for future attacks, considering learnings and adaptations to take from incidents

- **Digital Forensics Examiner**: work as part of a law-enforcement department, focused on collecting and analysing evidence to help solve crimes: charging the guilty and exonerating the innocent. On the other hand, if your work falls under defending a company's network, you will be using your forensic skills to analyse incidents, such as policy violations.

**Responsibilities**:
- Collect digital evidence while observing legal procedures
- Analyse digital evidence to find answers related to the case
- Document your findings and report on the case

- **Malware Analyst**: role is analysing suspicious programs, discovering what they do and writing reports about their findings. A malware analyst is sometimes called a reverse-engineer as their core task revolves around converting compiled programs from machine language to readable code, usually in a low-level language. This work requires the malware analyst to have a strong programming background, especially in low-level languages such as assembly language and C language. The ultimate goal is to learn about all the activities that a malicious program carries out, find out how to detect it and report it.

**Responsibilities**:
- Carry out static analysis of malicious programs, which entails reverse-engineering
- Conduct dynamic analysis of malware samples by observing their activities in a controlled environment
- Document and report all the findings

- **Penetration Tester**: role is to test the security of the systems and software within a company - this is achieved through attempts to uncover flaws and vulnerabilities through systemised hacking. Penetration testers exploit these vulnerabilities to evaluate the risk in each instance. The company can then take these insights to rectify issues to prevent a real-world cyberattack.

**Responsibilities**:
- Conduct tests on computer systems, networks, and web-based applications
- Perform security assessments, audits, and analyse policies
- Evaluate and report on insights, recommending actions for attack prevention

- **Red Teamer**: look to uncover many vulnerabilities across systems to keep cyber-defence in good standing, whilst red teamers are enacted to test the company's detection and response capabilities. This job role requires imitating cyber criminals' actions, emulating malicious attacks, retaining access, and avoiding detection. Red team assessments can run for up to a month, typically by a team external to the company. They are often best suited to organisations with mature security programs in place.

**Responsibilities**:
- Emulate the role of a threat actor to uncover exploitable vulnerabilities, maintain access and avoid detection
- Assess organisations' security controls, threat intelligence, and incident response procedures
- Evaluate and report on insights, with actionable data for companies to avoid real-world instances
# Module 2 - Network Fundamentals

## What is Networking?
Note: I completed this section on the free tier. The remaining sections in Module 2 (Intro to LAN, OSI Model, Packets & Frames, Extending Your Network) are behind a paywall so I haven't covered those yet.

What was the objective?

The objective of this section was to understand what a network actually is, why networks exist, and how devices communicate with each other on a basic level.

What did I learn?

I learned that a network is simply a group of connected devices that can communicate with each other and share resources. This could be as small as two computers connected at home, or as large as millions of devices connected across the internet.

I learned that the internet itself is just one giant network — it's basically a massive collection of smaller networks all joined together.

I also learned about the two types of networks:


LAN (Local Area Network): A smaller network that covers a limited area, like a home, school, or office building. For example, the devices in my house connected to the same Wi-Fi are all part of a LAN.
WAN (Wide Area Network): A much larger network that spans across large geographic areas. The internet is the biggest example of a WAN.


Another key thing I picked up was that every device on a network needs a way to be identified so data gets sent to the right place. This is done through IP addresses and MAC addresses:


IP Address: This is like a device's postal address on a network — it tells the network where to send data.
MAC Address: This is a unique identifier that is physically built into a device's network hardware. Unlike IP addresses, MAC addresses don't change.


I also learned about ping, which is a basic tool used to test whether one device can communicate with another on a network. It works by sending a small packet of data to a target device and waiting for a reply. If you get a reply, the connection works. If you don't, something is blocking it or the device is unreachable.

What I took away from this

This section gave me a solid foundation for understanding how devices talk to each other. Before this I kind of knew what Wi-Fi and the internet were, but I didn't really understand the structure behind it — like how every device has its own identity on a network, or that the internet is just a huge web of smaller networks. It clicked for me when I thought about it like a postal system — every device has an address, and data is the letter being delivered.
## Intro to LAN

## OSI Model

## Packets & Frames

## Extending Your Network

# Module 3 - How The Web Works

## DNS in Detail
Note: I completed this section on the free tier. The remaining sections in Module 3 (HTTP in Detail, How Websites Work, Putting it all together) are behind a paywall so I haven't covered those yet.




What was the objective?

The objective of this section was to understand what DNS is, how it works, and why it's essential to how we browse the internet every day.

What did I learn?

I learned that DNS stands for Domain Name System, and basically it's the internet's phonebook. Every website has an IP address (a string of numbers like 104.26.10.229), but instead of us having to memorise those numbers for every site we visit, DNS translates human-readable domain names like google.com into the IP address the computer actually needs to connect to it.

I learned that there are different types of DNS records, each serving a different purpose:


A Record: Maps a domain name to an IPv4 address. This is the most common one — it's what points example.com to an IP.
AAAA Record: Same as an A record but for IPv6 addresses, which are longer.
CNAME Record: Maps one domain to another domain instead of an IP. For example, www.example.com might point to example.com using a CNAME.
MX Record: Stands for Mail Exchange — it directs emails sent to a domain to the right mail server.
TXT Record: Stores text information. Often used for verification purposes, like proving you own a domain.


I also learned how the DNS lookup process actually works step by step:


I type a domain into my browser like tryhackme.com
My computer first checks its own local cache — if it's visited this site before, it might already know the IP
If not, it asks a Recursive DNS Server (usually provided by my ISP) which also checks its cache
If the recursive server doesn't know, it asks the Root DNS Servers — these are the top level and point toward the right direction
The root server points to the TLD (Top Level Domain) server for .com, .co.uk etc.
The TLD server then points to the Authoritative DNS Server for that specific domain, which holds the actual DNS records
The IP address is returned all the way back to my browser, and the connection is made


I also learned about TTL (Time to Live) — this is a value set on DNS records that tells other servers how long to cache that record before checking again. A short TTL means changes to DNS records take effect faster, but it also means more frequent lookups.

What I took away from this

Before this section I just took it for granted that typing a website name into a browser just worked. Now I actually understand the chain of servers working behind the scenes every time I visit a site. The thing that stuck with me most was the step-by-step lookup process — it's like asking multiple people for directions until you reach someone who knows the exact address.
## HTTP in Detail

## How Websites Work

## Putting it all together

# Module 4 - Computer Fundamentals

## Inside a Computer System
Note: I completed this section on the free tier. The remaining sections in Module 4 (Computer Types, Client-Server Basics, Virtualisation Basics, Cloud Computing Fundamentals) are behind a paywall so I haven't covered those yet.




What was the objective?

The objective of this section was to understand what components make up a computer system, what each one does, and how they all work together.

What did I learn?

I learned that a computer system is made up of several key hardware components, and each one plays a specific role in making the system function.

CPU (Central Processing Unit)
I learned that the CPU is basically the brain of the computer. It's responsible for processing instructions — every time you open an app, click something, or run a program, the CPU is the one doing the actual work of executing those instructions. The speed of a CPU is measured in GHz (gigahertz), and modern CPUs have multiple cores, meaning they can handle multiple tasks at the same time.

RAM (Random Access Memory)
RAM is the computer's short-term memory. It temporarily stores data that the CPU is actively using so it can be accessed quickly. The more RAM a computer has, the more it can handle at once without slowing down. Unlike storage, RAM is wiped every time the computer is turned off.

Storage (HDD / SSD)
This is the computer's long-term memory — where everything is saved permanently, like files, the operating system, and installed software. I learned about the two main types:


HDD (Hard Disk Drive): Uses spinning magnetic disks to store data. Slower but cheaper for large storage.
SSD (Solid State Drive): Uses flash memory with no moving parts. Much faster than an HDD, which is why computers with SSDs boot up significantly quicker.


Motherboard
I learned that the motherboard is what connects everything together. It's the main circuit board inside the computer that allows the CPU, RAM, storage, and other components to communicate with each other.

PSU (Power Supply Unit)
The PSU converts mains electricity into the lower voltages that the internal components of the computer actually need to operate.

GPU (Graphics Processing Unit)
The GPU handles the rendering of images, video, and animations. While the CPU handles general processing, the GPU is specialised for graphical tasks. This is especially important for gaming or video editing.

I also learned about the difference between input and output devices:


Input devices are things that send data into the computer — like a keyboard, mouse, or microphone.
Output devices are things the computer uses to send information out — like a monitor, speakers, or a printer.


What I took away from this

This section helped me understand what's actually inside a computer rather than just seeing it as a black box. The thing that clicked for me was the difference between RAM and storage — I used to think they were basically the same thing, but they serve completely different purposes. RAM is what the computer is actively thinking about right now, storage is everything it's got saved for later.
## Computer Types

## Client-Server Basics

## Virtualisation Basics

## Cloud Computing Fundamentals

# Module 5 - Operating System Basics

## Operating Systems: Introduction
Note: I completed this section on the free tier. The remaining sections in Module 5 (Windows Basics, Linux CLI Basics, Windows CLI Basics, Operating System Security) are behind a paywall so I haven't covered those yet.




What was the objective?

The objective of this section was to understand what an operating system actually is, what it does, and why it's essential for any computer to function.

What did I learn?

I learned that an Operating System (OS) is the software that manages all the hardware and software resources on a computer. Without an OS, the hardware wouldn't know what to do and you couldn't run any programs at all. It basically acts as the middleman between the user and the hardware.

The main jobs of an operating system are:


Process Management: The OS controls which programs are running and allocates CPU time to them. When I have multiple apps open at the same time, it's the OS managing how they all share the processor.
Memory Management: The OS decides how RAM is allocated between different running programs. It makes sure each program gets the memory it needs without crashing into another program's space.
File System Management: The OS organises how data is stored and retrieved on storage devices. It's what makes folders, files, and directories work the way they do.
Device Management: The OS communicates with hardware devices like printers, keyboards, and monitors through drivers. A driver is basically a translator between the OS and a piece of hardware.
Security and Access Control: The OS manages user accounts and permissions — deciding who can access what on the system.


I also learned about the different types of operating systems:


Desktop OS: Designed for personal computers — examples include Windows, macOS, and Linux.
Mobile OS: Designed for smartphones and tablets — examples include Android and iOS.
Server OS: Designed to manage and serve resources to other computers on a network — examples include Windows Server and Ubuntu Server.


Another key concept I picked up was the Kernel — this is the core part of the operating system that directly interacts with the hardware. Everything else in the OS sits on top of the kernel. It's essentially the lowest level of software running on a computer.

I also learned about the difference between a GUI (Graphical User Interface) and a CLI (Command Line Interface):


A GUI is the visual, point-and-click interface most people are used to — like Windows desktop with icons and windows.
A CLI is text-based — you type commands directly. It's more powerful and efficient once you know what you're doing, which is why most hacking tools and server management is done through a CLI.


What I took away from this

I already had some idea of what an operating system was just from using Windows every day, but I didn't really understand everything happening underneath. The part that stood out most to me was learning about the kernel — knowing that there's this core layer that directly talks to the hardware, and everything else is built on top of it, made it easier to understand why different OS types exist and why some tasks require more direct access to the system than others.
## Windows Basics

## Linux CLI Basics

## Windows CLI Basics

## Operating System Security

# Module 6 - Software Basics

## Data Representation
Note: I completed this section on the free tier. The remaining sections in Module 6 (Data Encoding, Python: Simple Demo, JavaScript: Simple Demo, Database SQL Basics) are behind a paywall so I haven't covered those yet.




What was the objective?

The objective of this section was to understand how computers actually store and represent data, since computers don't understand text, images, or numbers the same way humans do.

What did I learn?

I learned that computers only understand two states — on and off — which is represented as 1 and 0. This is called the binary number system, and it's the foundation of everything a computer does. Every piece of data — whether it's a text message, an image, a video, or a program — is ultimately stored as a sequence of 1s and 0s.

Bits and Bytes
I learned that a single bit is the smallest unit of data — it's just a 0 or a 1. Eight bits together make a byte. From there:


1,000 bytes = 1 Kilobyte (KB)
1,000 KB = 1 Megabyte (MB)
1,000 MB = 1 Gigabyte (GB)
1,000 GB = 1 Terabyte (TB)


Binary (Base-2)
I learned how binary numbers work. Unlike the decimal system we use every day (base-10, digits 0–9), binary only uses 0 and 1. Each position in a binary number represents a power of 2:

1286432168421

So the binary number 00001010 equals 8 + 2 = 10 in decimal. I found it useful to think of each column as a switch — if it's a 1, that value counts, if it's a 0, it doesn't.

Hexadecimal (Base-16)
I also learned about hexadecimal, which is a base-16 number system that uses digits 0–9 and then letters A–F to represent values 10–15. Hex is used a lot in computing because it's a more compact way of representing binary — 8 bits of binary can be written as just 2 hex digits. You see hexadecimal used in things like colour codes in web design (like #FF5733) and memory addresses.

How text is represented
I learned that text is stored using character encoding systems. The most well known is ASCII (American Standard Code for Information Interchange), which assigns a number to each letter, digit, and symbol. For example, the letter "A" is 65 in ASCII. The computer stores that number in binary, and when it displays it, it converts it back to the character.

What I took away from this

I always knew computers used binary at some level but I never really understood how it actually worked until this section. The thing that clicked for me was realising that everything — every file, every image, every piece of text — is just numbers under the hood, and binary is how those numbers are stored at the hardware level. Understanding hex also made sense of things I'd seen before but never understood, like colour codes in web design or memory addresses when debugging.
## Data Encoding

## Python: Simple Demo

## JavaScript: Simple Demo

## Database SQL Basics

# Module 7 - Attacks and Defenses

## The CIA Triad
Note: I completed this section on the free tier. The remaining sections in Module 7 (Cryptography Concepts, Become a Hacker, Become a Defender) are behind a paywall so I haven't covered those yet.




What was the objective?

The objective of this section was to understand the CIA Triad — the three core principles that form the foundation of cybersecurity.

What did I learn?

I learned that the CIA Triad stands for Confidentiality, Integrity, and Availability. These are the three fundamental goals that every security system, policy, and control is built around. If any one of these three is compromised, there's a security problem.

Confidentiality
Confidentiality is about making sure that information is only accessible to people who are authorised to see it. The goal is to prevent unauthorised access or disclosure of sensitive data.

Examples of how confidentiality is protected:


Encryption: Scrambling data so only someone with the right key can read it
Access controls: Making sure only the right people can access certain files or systems
Authentication: Verifying who someone is before granting them access — like passwords or two-factor authentication


A breach of confidentiality would be something like a hacker stealing a database of user passwords, or an employee leaking sensitive company information.

Integrity
Integrity is about making sure that data is accurate and hasn't been tampered with. It ensures that information is trustworthy and that any unauthorised changes are detected.

Examples of how integrity is maintained:


Hashing: A mathematical function that produces a unique fingerprint of data. If even one character in a file is changed, the hash changes — making tampering detectable
Digital signatures: Used to verify that a file or message came from who it says it came from and hasn't been altered
Checksums: Similar to hashing, used to verify data hasn't been corrupted during transfer


A breach of integrity would be something like an attacker modifying a financial record, or malware altering system files.

Availability
Availability is about making sure that systems, data, and services are accessible to authorised users when they need them. It doesn't matter how confidential or accurate your data is if nobody can get to it.

Examples of how availability is maintained:


Backups: Keeping copies of data so it can be restored if something goes wrong
Redundancy: Having backup systems that kick in if the main one fails
DDoS protection: Defending against Distributed Denial of Service attacks, where attackers flood a system with traffic to take it offline


A breach of availability would be something like a ransomware attack locking an organisation out of their own systems, or a DDoS attack taking down a website.

Why the CIA Triad matters
I learned that in cybersecurity, every attack can usually be linked back to a violation of one or more of these three principles. For example:


A data breach = Confidentiality failure
A man-in-the-middle attack altering messages = Integrity failure
A ransomware attack = Availability failure


Understanding the CIA Triad helps security professionals think about threats in a structured way — instead of reacting to individual attacks, you can ask: which of these three principles is being targeted, and how do I protect it?

What I took away from this

The CIA Triad gave me a proper framework for thinking about cybersecurity rather than just thinking about it as "stopping hackers." Every security decision — whether it's setting up a firewall, encrypting a file, or backing up data — maps back to one of these three goals. The one that surprised me most was Availability, because I hadn't really thought about it as a security concern before. But when I thought about how devastating a ransomware attack that locks you out of your own systems would be, it made complete sense why it's just as important as the other two.
## Cryptography Concepts

## Become a Hacker

## Become a Defender
