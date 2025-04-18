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


**Pass-around** reviews are often done via email or using a central code review system, allowing developers to review code asynchronously. 
**Pair programming** requires two programmers to work together, with one writing code and the other reviewing and
tracking progress. 
**Team reviews** are typically done in a group, 
**Fagan inspection** is a formal review process that would involve both the developer and a team to review the code using a formal process

---

**Multipartite viruses** use multiple propagation mechanisms to defeat system security controls but do not necessarily include techniques designed to hide the malware from antivirus software. 
**Stealth viruses** tamper with the operating system to hide their existence. 
**Polymorphic viruses** alter their code on each system they infect to defeat signature detection. 
**Encrypted viruses** use a similar technique, employing encryption to alter their appearance and avoid signature detection mechanisms.

---


## 🧾 Software requirements

| **Option**               | **Description**                                                                                  |
|--------------------------|--------------------------------------------------------------------------------------------------|
| **A. Derived Requirements**     | Requirements that are deduced or inferred from higher-level (parent) requirements. These support the main functional and non-functional requirements. |
| **B. Structural Requirements**  | Requirements that focus on the system's architecture, design, or how components are arranged, rather than how the system behaves. |
| **C. Behavioral Requirements**  | Describe **how** the system should behave in response to specific inputs or conditions. They often overlap with functional requirements but focus more on **system reactions**. |
| **D. Functional Requirements** | Define the **specific tasks**, **inputs**, **outputs**, and **interactions** the software must perform to meet user needs. |

---

**Lost updates** occur when one transaction writes a value to the database that overwrites a value needed by transactions that have earlier precedence, causing those transactions to read an incorrect value. 
**Dirty reads** occur when one transaction reads a value from a database that was written by another transaction that did not commit. 
**Incorrect summaries** occur when one transaction is using an aggregate function to summarize data stored in a database while a second transaction is making modifications to the database, causing the summary to include incorrect information. 
**SQL injection** is a web application security flaw, not a database concurrency problem

---

## 📊 Charts and Diagrams in Project & Software Management

| **Term**             | **Description**                                                                                          |
|----------------------|----------------------------------------------------------------------------------------------------------|
| **WBS Chart** (Work Breakdown Structure) | A hierarchical breakdown of the project into smaller tasks or deliverables. Useful for managing scope and assigning responsibilities. |
| **PERT Chart** (Program Evaluation Review Technique) | A network-based planning tool used to determine task sequences and calculate the project timeline using critical path analysis. |
| **Gantt Chart**      | A bar chart that displays the project schedule over time. Shows task durations, dependencies, and progress. |
| **Wireframe Diagram**| A low-fidelity layout of a web or app interface. Helps visualize user experience, page structure, and interactions. |

---


