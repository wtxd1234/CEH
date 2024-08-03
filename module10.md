### Module 10: Denial-of-Service (DoS) Attacks

#### 10.1 Introduction to Denial-of-Service (DoS) Attacks
- **Denial-of-Service (DoS) Attack**: An attack intended to disrupt the normal functioning of a targeted server, service, or network by overwhelming it with traffic or exploiting vulnerabilities.
- **Purpose**: To render a system or service unavailable to its intended users.

#### 10.2 Types of DoS Attacks
1. **Flood Attacks**
   - **Description**: Overwhelming a target with a flood of traffic or requests.
   - **Types**:
     - **ICMP Flood**: Sending a large number of ICMP packets (e.g., ping requests) to exhaust resources.
     - **SYN Flood**: Sending numerous SYN requests to a server, consuming its resources and causing it to be unable to process legitimate requests.
     - **UDP Flood**: Flooding the target with UDP packets, often causing it to run out of resources.
2. **Application Layer Attacks**
   - **Description**: Targeting specific applications or services to exhaust server resources.
   - **Types**:
     - **HTTP Flood**: Sending a large number of HTTP requests to a web server to consume resources.
     - **Slowloris**: Keeping many connections open and sending partial HTTP requests to tie up server resources.
3. **Distributed Denial-of-Service (DDoS) Attacks**
   - **Description**: A DoS attack executed from multiple systems or bots, making it more difficult to mitigate.
   - **Techniques**:
     - **Botnets**: Networks of compromised devices controlled by an attacker to perform coordinated attacks.
     - **Amplification Attacks**: Exploiting publicly accessible servers to amplify the attack traffic.
   - **Examples**: DNS amplification, NTP amplification.

#### 10.3 Tools for Performing DoS Attacks
1. **LOIC (Low Orbit Ion Cannon)**
   - **Description**: A popular tool used for performing DoS and DDoS attacks by flooding a target with traffic.
2. **HOIC (High Orbit Ion Cannon)**
   - **Description**: Similar to LOIC but capable of launching more sophisticated attacks with increased payloads.
3. **Hping**
   - **Description**: A command-line tool for crafting and sending custom packets, used for DoS testing and attacks.
4. **Slowloris**
   - **Description**: A tool that keeps many connections open to a web server by sending partial HTTP requests.

#### 10.4 Techniques for Executing DoS Attacks
1. **Bandwidth Exhaustion**
   - Consuming all available bandwidth to prevent legitimate users from accessing the network.
2. **Resource Exhaustion**
   - Depleting server resources such as CPU, memory, or disk space to disrupt service.
3. **Crash Attacks**
   - Exploiting vulnerabilities to crash services or applications.

#### 10.5 Countermeasures for DoS Attacks
1. **Rate Limiting**
   - Restricting the number of requests a user or IP address can make in a given timeframe.
2. **Traffic Filtering**
   - Using firewalls and intrusion prevention systems (IPS) to filter out malicious traffic.
3. **Load Balancing**
   - Distributing traffic across multiple servers to mitigate the impact of an attack.
4. **Content Delivery Network (CDN)**
   - Leveraging CDNs to absorb and mitigate attack traffic by distributing it across a network of servers.
5. **Anomaly Detection**
   - Implementing monitoring systems to detect and respond to unusual traffic patterns or behavior.
6. **IP Blacklisting**
   - Blocking traffic from IP addresses known to be involved in malicious activities.

#### 10.6 Mitigation Strategies
1. **Redundancy**
   - Ensuring redundancy in network and server infrastructure to maintain service availability during attacks.
2. **Scaling**
   - Scaling resources up or down to handle increased traffic loads and mitigate the effects of an attack.
3. **Incident Response Plan**
   - Developing and maintaining a response plan for DoS attacks to ensure quick and effective mitigation.

#### 10.7 Reporting DoS Attacks
- **Incident Documentation**: Recording details of the attack, including attack vectors, affected systems, and impact.
- **Impact Assessment**: Evaluating the damage caused by the attack, including service downtime and data loss.
- **Mitigation Actions**: Documenting the steps taken to mitigate the attack and restore service.
- **Post-Incident Review**: Analyzing the attack to improve defenses and response strategies.
