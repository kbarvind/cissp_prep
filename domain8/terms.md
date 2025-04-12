## 🤖 Botnet and Related Terms – CISSP Perspective

A **botnet** is a network of compromised devices (bots or zombies) that are infected with malicious software and remotely controlled by an attacker (botmaster). Botnets are a major cybersecurity concern and appear in multiple CISSP domains.

---

### 🔐 Relevance in CISSP Domains

| Domain | Area of Focus |
|--------|----------------|
| **Domain 1** – Security and Risk Management | Threat modeling, risk identification |
| **Domain 3** – Security Architecture and Engineering | Malware types and endpoint security |
| **Domain 6** – Security Assessment and Testing | Malware in pentesting scenarios |
| **Domain 7** – Security Operations | Incident response, malware monitoring |

---

### 🧠 Key Concepts and Related Terms

#### 1. **Zombie**
A device infected by malware and controlled remotely. Part of the botnet and used without the owner's consent.

---

#### 2. **Command and Control (C2 or C&C) Server**
The attacker's control point for sending commands to bots and receiving stolen data.

- Common protocols: HTTP, IRC, P2P, or even social media.

---

#### 3. **Bot Herder (Botmaster)**
The attacker or group that builds, maintains, and controls the botnet.

---

#### 4. **DDoS (Distributed Denial of Service)**
A common use of botnets where thousands of bots flood a target with traffic, making services unavailable.

---

#### 5. **Malware**
Software used to compromise and control machines. Botnets often start with:
- **Trojans**
- **Worms**
- **Rootkits**
- **Keyloggers**

---

#### 6. **Dropper**
A type of malware that delivers or installs other malware (e.g., botnet payloads) on a system.

---

#### 7. **Detection and Mitigation Techniques**

- **Network Monitoring**: Detect unusual outbound/inbound traffic.
- **Endpoint Detection and Response (EDR)**: Identifies malicious behavior on endpoints.
- **Firewalls, IDS/IPS**: Prevent and detect malicious connections.
- **Threat Intelligence Feeds**: Recognize known C2 IPs/domains.
- **Sinkholing**: Redirect malicious traffic to a controlled server to prevent real C2 communication.

---

#### 8. **Real-World Botnet Examples**

- **Mirai**: Targeted IoT devices for large-scale DDoS attacks.
- **Zeus/Zbot**: Stole banking credentials.
- **Emotet**: Malware platform used for spam and delivering other malware.

---