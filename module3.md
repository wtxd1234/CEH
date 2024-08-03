### Module 3: Scanning Networks

#### 3.1 Introduction to Network Scanning
- **Network Scanning**: The process of identifying active devices, open ports, and services on a network.
- **Purpose**: To discover network security vulnerabilities that can be exploited.

#### 3.2 Types of Network Scanning
1. **Port Scanning**
   - Identifies open ports and services available on a target host.
   - Determines the status of ports (open, closed, filtered).
2. **Vulnerability Scanning**
   - Identifies vulnerabilities in systems and applications.
   - Uses automated tools to scan for known security issues.
3. **Network Scanning**
   - Discovers devices and hosts on a network.
   - Identifies IP addresses and device types.

#### 3.3 Scanning Methodologies
- **Ping Sweep**: Identifies live hosts by sending ICMP echo requests.
- **Port Scan Types**:
  - **TCP Connect Scan**: Completes the TCP three-way handshake.
  - **SYN Scan**: Sends SYN packets and waits for responses without completing the handshake.
  - **FIN Scan**: Sends FIN packets to elicit a response from closed ports.
  - **XMAS Scan**: Sets the FIN, PSH, and URG flags in the TCP packet header.
  - **ACK Scan**: Determines firewall rulesets by sending ACK packets.
  - **UDP Scan**: Sends UDP packets to identify open UDP ports.

#### 3.4 Scanning Tools
- **Nmap**: A powerful open-source network scanner.
  - Features: Host discovery, port scanning, service enumeration, OS detection, scripting.
- **Angry IP Scanner**: A fast and simple network scanner.
- **Advanced IP Scanner**: Scans local networks and provides detailed information about network devices.
- **Netcat**: A versatile networking utility for reading from and writing to network connections.
- **Hping**: A network tool used for crafting TCP/IP packets and performing advanced network scanning.

#### 3.5 Interpreting Scan Results
- **Open Port**: A port that is accepting connections.
- **Closed Port**: A port that is accessible but not open for connections.
- **Filtered Port**: A port that is being filtered by a firewall or other security device, making it difficult to determine its status.

#### 3.6 Banner Grabbing
- **Banner Grabbing**: The process of capturing information about a service running on an open port.
- **Purpose**: To gather information about the software and version of services running on the target.

#### 3.7 OS Fingerprinting
- **Active OS Fingerprinting**: Sends crafted packets to the target and analyzes responses to determine the OS.
- **Passive OS Fingerprinting**: Analyzes traffic between the target and other systems to determine the OS.

#### 3.8 Scanning for Vulnerabilities
- **Automated Tools**: Nessus, OpenVAS, Nexpose.
- **Common Vulnerabilities**: Outdated software, misconfigurations, weak passwords, unpatched systems.

#### 3.9 Network Mapping
- **Network Mapping**: Creating a map of the network's topology.
- **Purpose**: To understand the structure of the network, including devices, connections, and paths.

#### 3.10 Countermeasures for Network Scanning
- **Firewall Configuration**: Blocking unnecessary ports and protocols.
- **Intrusion Detection Systems (IDS)**: Detecting and alerting on scanning activities.
- **Network Segmentation**: Dividing the network into segments to limit the spread of an attack.
- **Honeypots**: Deploying decoy systems to attract and monitor attackers.
- **Regular Updates and Patching**: Ensuring all systems and applications are up to date with the latest security patches.

#### 3.11 Reporting Scan Results
- **Documentation**: Recording all findings in a detailed report.
- **Analysis**: Highlighting critical vulnerabilities and providing an assessment of the risk.
- **Recommendations**: Offering remediation strategies to mitigate identified vulnerabilities.
