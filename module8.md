### Module 8: Sniffing

#### 8.1 Introduction to Sniffing
- **Sniffing**: The process of intercepting and capturing network traffic.
- **Purpose**: To analyze network traffic and extract sensitive information.

#### 8.2 Types of Sniffing
1. **Passive Sniffing**
   - Listening to network traffic without interfering with the network.
   - Suitable for environments with hubs or wireless networks.
2. **Active Sniffing**
   - Actively injecting traffic or performing actions to capture traffic.
   - Suitable for environments with switches.

#### 8.3 Network Protocols Vulnerable to Sniffing
1. **HTTP**: Transmits data in plaintext, making it vulnerable to interception.
2. **FTP**: Transmits credentials and data in plaintext.
3. **Telnet**: Transmits data in plaintext, including credentials.
4. **SMTP**: Transmits emails in plaintext.
5. **POP3/IMAP**: Transmits email data in plaintext.
6. **DNS**: Can be spoofed or redirected to capture traffic.

#### 8.4 Sniffing Techniques
1. **MAC Flooding**
   - Overloading a switch's CAM table to force it to behave like a hub, broadcasting traffic.
   - Tools: `macof` (part of the Dsniff suite).
2. **ARP Spoofing/Poisoning**
   - Sending fake ARP messages to associate the attacker's MAC address with the IP address of another host.
   - Tools: `arpspoof` (part of the Dsniff suite), Cain & Abel, Ettercap.
3. **DHCP Spoofing**
   - Setting up a rogue DHCP server to provide attacker-controlled IP addresses to clients.
   - Tools: `Yersinia`, `dhcpstarv`.
4. **DNS Poisoning**
   - Redirecting traffic by providing false DNS responses.
   - Tools: `dnsspoof` (part of the Dsniff suite).

#### 8.5 Sniffing Tools
1. **Wireshark**
   - A powerful and widely-used network protocol analyzer.
   - Features: Capturing and analyzing network traffic, protocol decoding, filtering.
2. **Tcpdump**
   - A command-line packet analyzer.
   - Features: Capturing and analyzing network traffic, filtering by protocols or addresses.
3. **Ettercap**
   - A comprehensive suite for man-in-the-middle attacks on LAN.
   - Features: ARP spoofing, password sniffing, traffic injection.
4. **Cain & Abel**
   - A password recovery tool that can also perform ARP poisoning and traffic sniffing.
   - Features: Password cracking, ARP spoofing, traffic capture.
5. **Dsniff**
   - A suite of tools for network auditing and penetration testing.
   - Tools: `dsniff`, `arpspoof`, `dnsspoof`, `filesnarf`, `mailsnarf`, `msgsnarf`, `urlsnarf`, `webspy`.

#### 8.6 Wireless Sniffing
- **Wireless Sniffing**: Capturing traffic on wireless networks.
- **Techniques**: Passive sniffing (monitor mode), active sniffing (deauthentication attacks).
- **Tools**: Aircrack-ng suite (Airodump-ng, Aircrack-ng, Aireplay-ng).

#### 8.7 Countermeasures for Sniffing
1. **Encryption**
   - Using encryption protocols (e.g., HTTPS, SSH, VPN) to protect data in transit.
2. **Network Segmentation**
   - Segmenting the network to limit traffic exposure.
3. **Static ARP Entries**
   - Using static ARP entries to prevent ARP spoofing.
4. **Port Security**
   - Configuring switches to limit the number of MAC addresses per port.
5. **Monitoring and Detection**
   - Using IDS/IPS to detect and alert on sniffing activities.
   - Tools: Snort, Suricata.
6. **Educating Users**
   - Training users on the importance of using secure communication channels and recognizing suspicious activities.

#### 8.8 Reporting Sniffing Activities
- **Documentation**: Keeping detailed records of detected sniffing activities and associated evidence.
- **Impact Assessment**: Evaluating the potential impact of sniffing on the organization's security.
- **Mitigation Recommendations**: Providing actionable steps to mitigate sniffing threats and enhance network security.
- **Verification of Mitigations**: Ensuring that recommended security measures are implemented and effective.
