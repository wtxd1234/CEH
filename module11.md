### Module 11: Session Hijacking

#### 11.1 Introduction to Session Hijacking
- **Session Hijacking**: The exploitation of a valid computer session to gain unauthorized access to a web application or network.
- **Purpose**: To steal or impersonate an active session to perform actions as if you were the legitimate user.

#### 11.2 Types of Session Hijacking
1. **Session Fixation**
   - **Description**: Attacker sets a known session ID for the victim before the victim logs in, allowing the attacker to hijack the session once the victim authenticates.
   - **Techniques**: Embedding a fixed session ID in URLs, cookies.
2. **Session Prediction**
   - **Description**: Attacker predicts or guesses valid session IDs to hijack sessions.
   - **Techniques**: Analyzing session ID patterns, using brute-force methods.
3. **Session Sidejacking**
   - **Description**: Intercepting unencrypted session cookies over the network.
   - **Techniques**: Using packet sniffers to capture session cookies from network traffic.
4. **Session Sniffing**
   - **Description**: Capturing session cookies or tokens transmitted over the network.
   - **Tools**: Wireshark, tcpdump.
5. **Cross-Site Scripting (XSS)**
   - **Description**: Exploiting XSS vulnerabilities to steal session cookies or tokens.
   - **Techniques**: Injecting malicious scripts into web pages to capture cookies.

#### 11.3 Tools for Session Hijacking
1. **Ettercap**
   - **Description**: A network sniffing tool that supports session hijacking and Man-in-the-Middle (MitM) attacks.
2. **Firebug and Web Developer Tools**
   - **Description**: Browser plugins used for inspecting cookies, headers, and session data.
3. **Hamster and Ferret**
   - **Description**: Tools for capturing and replaying HTTP cookies to perform session hijacking.

#### 11.4 Techniques for Session Hijacking
1. **Session Cookie Theft**
   - Capturing cookies used for session management.
   - Tools: Sniffing tools, XSS attacks.
2. **Session Token Theft**
   - Capturing tokens used to authenticate sessions.
   - Techniques: Sniffing, predicting, or injecting tokens.
3. **Session Replay**
   - Replaying captured session tokens or cookies to gain unauthorized access.

#### 11.5 Countermeasures for Session Hijacking
1. **Use HTTPS**
   - Encrypting data transmitted between clients and servers to protect session cookies from being intercepted.
2. **Secure Session Cookies**
   - Implementing the `Secure` and `HttpOnly` flags on cookies to prevent them from being accessed or transmitted over insecure channels.
   - Techniques: Setting `Secure` flag to ensure cookies are only sent over HTTPS, and `HttpOnly` flag to prevent JavaScript access.
3. **Session Timeouts**
   - Setting session timeouts to reduce the window of opportunity for session hijacking.
4. **Session Regeneration**
   - Regenerating session IDs after login and other critical actions to prevent session fixation attacks.
5. **Input Validation and Sanitization**
   - Validating and sanitizing user input to prevent XSS attacks that could be used to steal session cookies.
6. **Multi-Factor Authentication (MFA)**
   - Implementing MFA to add an additional layer of security beyond session cookies or tokens.
7. **Regular Monitoring**
   - Monitoring session activity for unusual behavior or unauthorized access attempts.

#### 11.6 Reporting Session Hijacking Incidents
- **Incident Documentation**: Recording the details of the session hijacking attack, including affected users, methods used, and impact.
- **Impact Assessment**: Evaluating the effects of the attack on the organization’s security and user data.
- **Mitigation Actions**: Documenting the steps taken to mitigate the attack and secure sessions.
- **Post-Incident Review**: Analyzing the attack to improve session security and prevent future incidents.
