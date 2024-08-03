### Module 6: System Hacking

#### 6.1 Introduction to System Hacking
- **System Hacking**: The process of compromising individual systems to gain unauthorized access to data or resources.
- **Purpose**: To understand how attackers operate and to develop strategies to defend against such attacks.

#### 6.2 Goals of System Hacking
1. **Gaining Access**
   - Obtaining initial access to the target system.
2. **Escalating Privileges**
   - Increasing access rights to gain administrative or root privileges.
3. **Executing Applications**
   - Running malicious programs or scripts on the target system.
4. **Hiding Presence**
   - Ensuring that the attack remains undetected by cleaning logs and hiding traces.
5. **Creating Backdoors**
   - Setting up methods to regain access to the system later.

#### 6.3 Techniques for Gaining Access
1. **Password Cracking**
   - Techniques: Dictionary attacks, brute force attacks, and hybrid attacks.
   - Tools: John the Ripper, Hashcat, Hydra.
2. **Social Engineering**
   - Techniques: Phishing, pretexting, baiting, and tailgating.
3. **Exploiting Vulnerabilities**
   - Using known vulnerabilities in software to gain access.
   - Tools: Metasploit, Core Impact, Exploit DB.
4. **Keyloggers**
   - Capturing keystrokes to steal passwords and sensitive information.
   - Tools: Keylogger software (e.g., Spyrix Keylogger, KidLogger).

#### 6.4 Techniques for Escalating Privileges
1. **Privilege Escalation Exploits**
   - Exploiting vulnerabilities in the operating system or applications to gain higher privileges.
   - Tools: Metasploit, local exploit scripts.
2. **Password Cracking**
   - Cracking administrator or root passwords to gain elevated privileges.
3. **Buffer Overflow**
   - Exploiting buffer overflow vulnerabilities to execute arbitrary code with elevated privileges.

#### 6.5 Techniques for Executing Applications
1. **Remote Code Execution**
   - Executing commands or scripts on the target system remotely.
   - Tools: Metasploit, PsExec.
2. **Scheduled Tasks**
   - Creating scheduled tasks to execute malicious programs.
   - Tools: Windows Task Scheduler, `cron` jobs in Unix/Linux.

#### 6.6 Techniques for Hiding Presence
1. **Clearing Logs**
   - Deleting or altering system logs to remove evidence of the attack.
   - Tools: `wevtutil` (Windows), `shred` (Linux), log cleaners.
2. **Rootkits**
   - Installing rootkits to hide malicious processes and files.
   - Tools: `Hacker Defender`, `GrayFish`.
3. **Steganography**
   - Hiding data within other non-suspicious files (e.g., images, audio files).
   - Tools: Steghide, OpenPuff.

#### 6.7 Techniques for Creating Backdoors
1. **Backdoor Tools**
   - Installing backdoor programs to maintain persistent access.
   - Tools: Netcat, Metasploit’s Meterpreter, Remote Access Trojans (RATs) like DarkComet.
2. **Trojanizing Applications**
   - Embedding backdoors in legitimate applications or files.
   - Techniques: Wrappers, binders, Trojans.

#### 6.8 Covering Tracks
- **Log Tampering**: Modifying or deleting logs to remove evidence.
- **Time Stomping**: Changing timestamps of files to obscure evidence.
- **Alternate Data Streams**: Hiding data in NTFS alternate data streams.

#### 6.9 Tools for System Hacking
- **Password Cracking Tools**: John the Ripper, Hashcat, Cain & Abel.
- **Privilege Escalation Tools**: Metasploit, Windows Elevation of Privilege (EoP) exploits.
- **Rootkit Tools**: Hacker Defender, GrayFish.
- **Backdoor Tools**: Netcat, Meterpreter, DarkComet.

#### 6.10 Countermeasures for System Hacking
- **Strong Password Policies**: Enforcing complex passwords and regular password changes.
- **Patch Management**: Keeping systems and applications updated with the latest security patches.
- **User Education**: Training users to recognize social engineering attacks and practice good security hygiene.
- **Intrusion Detection Systems (IDS)**: Deploying IDS to detect and alert on suspicious activities.
- **Least Privilege Principle**: Granting users the minimum privileges necessary for their roles.
- **Regular Audits**: Conducting regular security audits and vulnerability assessments.
- **Anti-Malware Software**: Using and regularly updating anti-malware solutions to detect and remove malicious software.

#### 6.11 Reporting System Hacking Activities
- **Detailed Documentation**: Keeping detailed records of all activities, tools used, and findings.
- **Risk Assessment**: Evaluating the impact of identified vulnerabilities and attacks.
- **Mitigation Recommendations**: Providing actionable recommendations to remediate vulnerabilities and improve security.
- **Verification of Mitigations**: Ensuring that recommended security measures are implemented and effective.
