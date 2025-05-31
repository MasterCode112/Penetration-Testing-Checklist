# Penetration-Testing-Checklist
## Information Gathering

- [ ]  Manually explore the site
- [ ]  Spider/crawl for missed or hidden content
- [ ]  Check for files that expose content, such as `robots.txt`, `sitemap.xml`, `.DS_Store`
- [ ]  Check the caches of major search engines for publicly accessible sites
- [ ]  Check for differences in content based on User Agent (e.g., Mobile sites, access as a Search engine Crawler)
- [ ]  Perform Web Application Fingerprinting
- [ ]  Identify technologies used
- [ ]  Identify user roles
- [ ]  Identify application entry points
- [ ]  Identify client-side code
- [ ]  Identify multiple versions/channels (e.g., web, mobile web, mobile app, web services)
- [ ]  Identify co-hosted and related applications
- [ ]  Identify all hostnames and ports
- [ ]  Identify third-party hosted content

## Configuration Management

- [ ]  Check for commonly used application and administrative URLs
- [ ]  Check for old, backup, and unreferenced files
- [ ]  Check HTTP methods supported and Cross Site Tracing (XST)
- [ ]  Test file extensions handling
- [ ]  Test for security HTTP headers (e.g., CSP, X-Frame-Options, HSTS)
- [ ]  Test for policies (e.g., Flash, Silverlight, robots)
- [ ]  Test for non-production data in the live environment, and vice-versa
- [ ]  Check for sensitive data in client-side code (e.g., API keys, credentials)

## Secure Transmission

- [ ]  Check SSL Version, Algorithms, Key length
- [ ]  Check for Digital Certificate Validity (Duration, Signature, and CN)
- [ ]  Check credentials are only delivered over HTTPS
- [ ]  Check that the login form is delivered over HTTPS
- [ ]  Check session tokens are only delivered over HTTPS
- [ ]  Check if HTTP Strict Transport Security (HSTS) is in use

## Improved check list Additional Details

- [ ]  Hyper link
- [ ]  Reset links
- [ ]  Polices files (links)
- [ ]  new

## Authentication

- [ ]  Test for user enumeration
- [ ]  Test for authentication bypass
- [ ]  Test for bruteforce protection
- [ ]  Test password quality rules
- [ ]  Test remember me functionality
- [ ]  Test for autocomplete on password forms/input
- [ ]  Test password reset and/or recovery
- [ ]  Test password change process
- [ ]  Test CAPTCHA
- [ ]  Test multi-factor authentication
- [ ]  Test for logout functionality presence
- [ ]  Test for cache management on HTTP (e.g., Pragma, Expires, Max-age)
- [ ]  Test for default logins
- [ ]  Test for user-accessible authentication history
- [ ]  Test for out-of-channel notification of account lockouts and successful password changes
- [ ]  Test for consistent authentication across applications with shared authentication schema / SSO

## Session Management

- [ ]  Establish how session management is handled in the application (e.g., tokens in cookies, token in URL)
- [ ]  Check session tokens for cookie flags (httpOnly and secure)
- [ ]  Check session cookie scope (path and domain)
- [ ]  Check session cookie duration (expires and max-age)
- [ ]  Check session termination after a maximum lifetime
- [ ]  Check session termination after relative timeout
- [ ]  Check session termination after logout
- [ ]  Test to see if users can have multiple simultaneous sessions
- [ ]  Test session cookies for randomness
- [ ]  Confirm that new session tokens are issued on login, role change, and logout
- [ ]  Test for consistent session management across applications with shared session management
- [ ]  Test for session puzzling
- [ ]  Test for CSRF and clickjacking

## Authorization

- [ ]  Test for path traversal
- [ ]  Test for bypassing authorization schema
- [ ]  Test for vertical access control problems (a.k.a. Privilege Escalation)
- [ ]  Test for horizontal access control problems (between two users at the same privilege level)
- [ ]  Test for missing authorization

## Data Validation

- [ ]  Test for Reflected Cross Site Scripting
- [ ]  Test for Stored Cross Site Scripting
- [ ]  Test for DOM-based Cross Site Scripting
- [ ]  Test for Cross Site Flashing
- [ ]  Test for HTML Injection
- [ ]  Test for SQL Injection
- [ ]  Test for SOQL Injection
- [ ]  Test for LDAP Injection
- [ ]  Test for ORM Injection
- [ ]  Test for XML Injection
- [ ]  Test for XXE Injection
- [ ]  Test for SSI Injection
- [ ]  Test for XPath Injection
- [ ]  Test for XQuery Injection
- [ ]  Test for IMAP/SMTP Injection
- [ ]  Test for Code Injection
- [ ]  Test for Expression Language Injection
- [ ]  Test for Command Injection
- [ ]  Test for Overflow (Stack, Heap, and Integer)
- [ ]  Test for Format String
- [ ]  Test for incubated vulnerabilities
- [ ]  Test for HTTP Splitting/Smuggling
- [ ]  Test for HTTP Verb Tampering
- [ ]  Test for Open Redirection
- [ ]  Test for Local File Inclusion
- [ ]  Test for Remote File Inclusion
- [ ]  Compare client-side and server-side validation rules
- [ ]  Test for NoSQL injection
- [ ]  Test for HTTP parameter pollution
- [ ]  Test for auto-binding
- [ ]  Test for Mass Assignment
- [ ]  Test for NULL/Invalid Session Cookie

## Denial of Service

- [ ]  Test for anti-automation
- [ ]  Test for account lockout
- [ ]  Test for HTTP protocol DoS
- [ ]  Test for SQL wildcard DoS

## Business Logic

- [ ]  Test for feature misuse
- [ ]  Test for lack of non-repudiation
- [ ]  Test for trust relationships
- [ ]  Test for integrity of data
- [ ]  Test segregation of duties

## Cryptography

- [ ]  Check if data which should be encrypted is not
- [ ]  Check for wrong algorithms usage depending on context
- [ ]  Check for weak algorithms usage
- [ ]  Check for proper use of salting
- [ ]  Check for randomness functions

## Risky Functionality - File Uploads

- [ ]  Test that acceptable file types are whitelisted
- [ ]  Test that file size limits, upload frequency, and total file counts are defined and enforced
- [ ]  Test that file contents match the defined file type
- [ ]  Test that all file uploads have Anti-Virus scanning in-place
- [ ]  Test that unsafe filenames are sanitized
- [ ]  Test that uploaded files are not directly accessible within the web root
- [ ]  Test that uploaded files are not served on the same hostname/port
- [ ]  Test that files and other media are integrated with the authentication and authorization schemas

## Risky Functionality - Card Payment

- [ ]  Test for known vulnerabilities and configuration issues on Web Server and Web Application
- [ ]  Test for default or guessable password
- [ ]  Test for non-production data in live environment, and vice-versa
- [ ]  Test for Injection vulnerabilities
- [ ]  Test for Buffer Overflows
- [ ]  Test for Insecure Cryptographic Storage
- [ ]  Test for Insufficient Transport Layer Protection
- [ ]  Test for Improper Error Handling
- [ ]  Test for all vulnerabilities with a CVSS v2 score > 4.0
- [ ]  Test for Authentication and Authorization issues
- [ ]  Test for CSRF

## HTML 5

- [ ]  Test Web Messaging
- [ ]  Test for Web Storage SQL injection
- [ ]  Check CORS implementation
- [ ]  Check Offline Web Application

Source: OWASP

## RESOURCES

### Sites

| Name                                 | Description                                                | URL                                                                          |
| ------------------------------------ | ---------------------------------------------------------- | ---------------------------------------------------------------------------- |
| **Hack The Box**                     | Realistic labs, challenges, AD, Android, Web, Crypto, etc. | [https://www.hackthebox.com](https://www.hackthebox.com/)                    |
| **TryHackMe**                        | Guided, beginner-to-advanced labs (Windows, Linux, etc.)   | [https://tryhackme.com](https://tryhackme.com/)                              |
| **VulnHub**                          | Downloadable vulnerable VMs (Boot2Root, CTF style)         | [https://www.vulnhub.com](https://www.vulnhub.com/)                          |
| **CyberSecLabs**                     | Hands-on labs for red team & blue team                     | [https://www.cyberseclabs.co.uk](https://www.cyberseclabs.co.uk/)            |
| **PentesterLab**                     | Real-world web app and API exploits (XSS, IDOR, JWT)       | [https://pentesterlab.com](https://pentesterlab.com/)                        |
| **PortSwigger Web Security Academy** | Best for Web (XSS, CSRF, SSRF, etc.)                       | [https://portswigger.net/web-security](https://portswigger.net/web-security) |
### Online Vulnerable Websites

These are web-based platforms accessible directly via a browser, ideal for practicing web application vulnerabilities like SQL injection, XSS, CSRF, and more.
1. **Acunetix Vulnweb Test Sites**
    - **URL**:
        - [http://testphp.vulnweb.com/](http://testphp.vulnweb.com/) (PHP, MySQL, Apache)
        - [http://testasp.vulnweb.com/](http://testasp.vulnweb.com/) (ASP)
        - [http://testaspnet.vulnweb.com/](http://testaspnet.vulnweb.com/) (ASP.NET)
        - [http://testhtml5.vulnweb.com/](http://testhtml5.vulnweb.com/) (HTML5, Nginx, Python, Flask, CouchDB)

2. **bWAPP (Buggy Web Application)**
	- **URL**: [http://bwapp.ywnxs.com/](http://bwapp.ywnxs.com/) (or download from [http://www.itsecgames.com/](http://www.itsecgames.com/))
	- **Description**: A free, open-source PHP/MySQL web application with over 100 vulnerabilities, covering the OWASP Top 10 (e.g., SQL injection, XSS, CSRF). Supports Linux/Windows with LAMP/WAMP/XAMPP or a pre-installed VM (bee-box).
	- **Use Case**: Ideal for beginners and advanced testers to practice web vulnerabilities with customizable security levels.

3. **OWASP Juice Shop**
	- **URL**: [https://owasp-juice-shop.herokuapp.com/](https://owasp-juice-shop.herokuapp.com/) (or download from [https://owasp.org/www-project-juice-shop/](https://owasp.org/www-project-juice-shop/))
	- **Description**: An open-source, modern web application written in Node.js, Express, and Angular. Contains a vast number of hacking challenges covering OWASP Top 10 vulnerabilities and more. Can be run locally or accessed online.
	- **Use Case**: Suitable for all skill levels, with challenges ranging from basic to advanced.
  
  4. **Google Gruyere** --> Tagert
	- **URL**: [http://google-gruyere.appspot.com/start](http://google-gruyere.appspot.com/start)
	- **Description**: A Python-based web application hosted on Google App Engine, designed for beginners. Includes vulnerabilities like XSS, CSRF, information disclosure, and remote code execution. Features a “cheesy” design and guided challenges.
	- **Use Case**: Great for learning basic web exploitation techniques.

5. **Hack This Site**
	- **URL**: [https://www.hackthissite.org/](https://www.hackthissite.org/)
	- **Description**: A free platform offering a variety of challenges, including basic, realistic, application, and JavaScript missions. Includes a vibrant community and forums for discussion.
	- **Use Case**: Suitable for beginners and intermediate testers, with a focus on real-world scenarios.

6. **Defend The Web (formerly Hack This)**
	- **URL**: [https://defendtheweb.net/](https://defendtheweb.net/)
	- **Description**: An interactive platform with challenges focused on web security, including XSS, SQL injection, and authentication flaws. Offers a gamified experience with community forums.
	- **Use Case**: Ideal for learning through interactive, hands-on challenges.

7. **Hack Yourself First**
	- **URL**: [http://hack-yourself-first.com/](http://hack-yourself-first.com/)
	- **Description**: An ASP.NET-based web application simulating real-world vulnerabilities like SQL injection, XSS, and authentication flaws. Designed to teach developers and testers how to find and fix security issues.
	- **Use Case**: Useful for developers and pentesters focusing on ASP.NET environments.

8. **Altoro Mutual**
	- **URL**: [http://demo.testfire.net/](http://demo.testfire.net/)
	- **Description**: A deliberately insecure online banking application (ASP.NET) simulating financial services. Includes vulnerabilities like SQL injection, XSS, and authentication flaws.
	- **Use Case**: Ideal for testing financial application security scenarios.

9. **Pentest Ground*
	- **URL**: [https://pentest-ground.com/](https://pentest-ground.com/)
	- **Description**: A free, deliberately vulnerable platform for practicing real-world exploitation techniques. Offers a playground for hackers and learners to test web vulnerabilities.
	- **Use Case**: Suitable for practicing modern web exploitation in a realistic environment.
	
10. **Webscantest**
	- **URL**: [http://www.webscantest.com/](http://www.webscantest.com/)
	- **Description**: A test site with vulnerabilities like SQL injection, XSS, and CSRF, designed for practicing web scanning and manual pentesting.
	- **Use Case**: Good for testing vulnerability scanners and manual techniques.


### Offline Vulnerable Web Applications

These require local setup (e.g., via Docker, VM, or LAMP/WAMP/XAMPP) and are ideal for controlled environments.

1. **Damn Vulnerable Web Application (DVWA)**
	- **Download**: [https://dvwa.co.uk/](https://dvwa.co.uk/) or GitHub[](https://github.com/digininja/DVWA)
	- **Description**: A PHP/MySQL web application with vulnerabilities categorized by difficulty (low, medium, high). Covers SQL injection, XSS, CSRF, command injection, and more. Requires XAMPP or similar. Source code is public for learning.
	- **Use Case**: Perfect for beginners to advanced testers, with adjustable security levels.

2. **OWASP Mutillidae II**
	- **Download**: [https://sourceforge.net/projects/mutillidae/](https://sourceforge.net/projects/mutillidae/) or pre-installed on SamuraiWTF, Metasploitable 2
	- **Description**: A free, open-source PHP web application with over 40 vulnerabilities, including OWASP Top 10 (e.g., SQL injection, XSS, HTML injection). Supports LAMP/WAMP/XAMPP. Offers hints for beginners.
	- **Use Case**: Ideal for learning and practicing web security with guided challenges.

3. **WebGoat**
	- **Download**: [https://owasp.org/www-project-webgoat/](https://owasp.org/www-project-webgoat/) (Java-based, version 8.0)
	- **Description**: An OWASP project, WebGoat is a Java-based insecure application with tutorials and lessons on vulnerabilities like XSS, SQL injection, and access control issues. Available as a JAR file or Docker image.
	- **Use Case**: Great for developers and testers learning secure coding and exploitation.

4. **BadStore**
	- **Download**: [http://badstore.net/](http://badstore.net/) or via GitHub
	- **Description**: A vulnerable web application demonstrating common e-commerce vulnerabilities like SQL injection and XSS. Designed to show how hackers exploit web flaws.
	- **Use Case**: Suitable for beginners practicing e-commerce security testing.

5. **BodgeIt Store**
	- **Download**: [https://github.com/psiinon/bodgeit](https://github.com/psiinon/bodgeit)
	- **Description**: A simple, vulnerable e-commerce web application (Java-based) with vulnerabilities like SQL injection, XSS, and CSRF. Easy to set up and aimed at beginners.
	- **Use Case**: Ideal for new pentesters focusing on e-commerce platforms.

### Vulnerable Virtual Machines (VMs)
These are complete systems with multiple vulnerable applications, ideal for network and web pentesting.

1. **Metasploitable 2**
    - **Download**: [https://sourceforge.net/projects/metasploitable/](https://sourceforge.net/projects/metasploitable/)
    - **Description**: A Linux-based VM with vulnerable services and web applications (e.g., Mutillidae, DVWA). Integrates with Metasploit Framework for exploit practice. Includes network and system vulnerabilities.
    - **Use Case**: Comprehensive pentesting practice for web and network attacks.
2. **VulnHub**
    - **URL**: [https://www.vulnhub.com/](https://www.vulnhub.com/)
    - **Description**: A platform offering hundreds of downloadable vulnerable VMs, each with unique challenges (e.g., web apps, network services). Examples include “Kioptrix” and “FristiLeaks.”
    - **Use Case**: Advanced practice for network and web pentesting in realistic scenarios.
3. **Web Security Dojo**
    - **Download**: [https://sourceforge.net/projects/websecuritydojo/](https://sourceforge.net/projects/websecuritydojo/)
    - **Description**: A self-contained VM with vulnerable web applications (e.g., WebGoat, DVWA) and tools like Burp Suite. Designed for web security training.
    - **Use Case**: Complete training environment for web pentesting.

### Additional Platforms

These are gamified or community-driven platforms for broader pentesting practice.

1. **Hack The Box**
    - **URL**: [https://www.hackthebox.com/](https://www.hackthebox.com/)
    - **Description**: A massive online platform with vulnerable machines, web apps, and challenges. Includes CTF-style scenarios and a large community. Requires VPN connection.
    - **Use Case**: Advanced pentesting practice for all skill levels.
2. **TryHackMe**
    - **URL**: [https://tryhackme.com/](https://tryhackme.com/)
    - **Description**: A beginner-friendly platform with prebuilt courses and vulnerable machines hosted in the cloud. Covers web, network, and system pentesting.
    - **Use Case**: Ideal for structured learning and hands-on practice.
3. **Root Me**
    - **URL**: [https://www.root-me.org/](https://www.root-me.org/)
    - **Description**: Offers over 400 challenges across web, network, forensics, and cryptography. Includes realistic scenarios and a practical approach to pentesting.
    - **Use Case**: Comprehensive platform for all pentesting domains.
4. **CTFlearn**
    - **URL**: [https://ctflearn.com/](https://ctflearn.com/)
    - **Description**: A beginner-friendly Capture The Flag (CTF) platform with challenges in web, forensics, crypto, and more. Community-driven with over 70,000 users.
    - **Use Case**: Great for CTF-style learning and competition.
5. **PortSwigger Web Security Academy**
    - **URL**: [https://portswigger.net/web-security](https://portswigger.net/web-security)
    - **Description**: A free platform by the creators of Burp Suite, offering labs and learning materials for web vulnerabilities like XSS, SQL injection, and CSRF.
    - **Use Case**: Focused web security training with practical labs.

### Recommendations for Safe Practice
- **Use a Virtual Machine**: Run offline applications or VMs in a virtualized environment (e.g., VMware, VirtualBox) to avoid risking your main system.
- **Isolate Your Environment**: Use a dedicated network or VPN to prevent accidental interaction with production systems.
- **Check Legal Scope**: Always verify the terms of service for each platform to ensure your testing is authorized.
- **Learn Secure Coding**: Use these platforms to understand vulnerabilities and how to mitigate them in development.
- **Community Resources**: Engage with communities on Hack The Box, TryHackMe, or Hellbound Hackers for tips and collaboration.


## Contact = 0765458977/dvdgodbless111@gmail.com
