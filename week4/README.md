
# Cybersecurity Internship – NetworkWalks

This repository documents the practical tasks, exercises, tools, and reports completed during my **Virtual Cybersecurity Internship at NetworkWalks**.

## Weekly Tasks

### Week 1 – Linux & Network Fundamentals
- Installed and configured Kali Linux in a Virtual Machine.
- Created and configured a local network (`10.0.0.0`).
- Practiced network traffic analysis using Wireshark.

### Week 2 – Network Scanning & Reconnaissance
- Discovered active network hosts using Zenmap.
- Identified IP and MAC addresses of network devices.
- Performed website and domain reconnaissance on NetworkWalks using:
  - cURL
  - DNSRecon
  - Wafw00f
  - WHOIS
  - WhatWeb
- Discovery via theHarvester
- Used Google Hacking Database (GHDB)
- Documented findings and prepared a technical report.

### Week 3 – Password Cracking & Hash Analysis
- Installed and configured **John the Ripper (JTR)** along with its GUI frontend, **Johnny**.
- Extracted password hashes from provided PDF files using **OnlineHashCrack**.
- Executed dictionary/cracking attacks on the extracted hashes using Johnny to recover the passwords.
- Practiced additional hash generation and password cracking using **NetworkWalks** online tools.

### Week 4 – Web Application Penetration Testing & Exploitation
- Performed a full web application security assessment against the target domain (`https://medirozahospital.com`) to complete four core objectives: locating confidential patient reports, cracking document passwords, extracting internal financial/shareholder records, and compiling a final report.
- **SQL Injection & Authentication Bypass:**
  - Inspected and tested the **Patient Portal** login interface for input validation flaws.
  - Exploited an **SQL Injection (SQLi)** vulnerability to bypass login authentication and gain unauthorized access to **3 confidential patient report PDFs**.
- **PDF Password Cracking:**
  - Extracted hashes and cracked the passwords for all three protected PDF reports using **NetworkWalks** online hash calculation and password cracking tools.
  - Successfully cracked **2 PDFs** using the default built-in wordlist provided on the platform.
  - Successfully cracked the **3rd PDF** by uploading a custom **John the Ripper** wordlist.
- **Directory Enumeration & Database Exposure:**
  - Queried the target's `robots.txt` file using `cURL` (`curl https://medirozahospital.com`) to identify restricted paths, uncovering the disallowed `/old/` directory.
  - Navigated to the `/old/` directory and discovered an exposed `.sql` database backup file.
  - Analyzed the SQL dump to extract sensitive organizational data, including **all staff salary records** and **shareholder details**.
- **Reporting & Documentation:**
  - Compiled all methodologies, proof-of-concept steps, discovered vulnerabilities, and extracted findings into a complete, structured penetration testing report.
