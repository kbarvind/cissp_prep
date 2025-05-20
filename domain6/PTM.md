
## NMAP Port Status:

- **Open:** The port is accessible on the remote system and an application is accepting connections on that port.
- **Closed:** The port is accessible on the remote system, but no application is accepting connections on that port.
- **Filtered:** The port is not accessible on the remote system.

---

WPA2-Enterprise because it uses 802.1X authentication instead of a shared key

---

## Key Functions of Aircrack-ng

| **Aircrack-ng Tool** | **Function** | **Purpose** |
|----------------------|-------------|------------|
| **Airmon-ng**  | Enable Monitor Mode | Puts the wireless adapter into **monitor mode** to capture packets. |
| **Airodump-ng** | Packet Capture | Captures and analyzes **Wi-Fi traffic**, including SSID, MAC addresses, signal strength, encryption type, and connected clients. |
| **Aircrack-ng** | Password Cracking | Performs **dictionary/brute-force attacks** on **WPA/WPA2 handshakes** to recover Wi-Fi passwords. |
| **Aireplay-ng** | Packet Injection & Deauthentication | Injects packets into a Wi-Fi network to **force deauthentication** of a client and capture the handshake. |
| **Airbase-ng**  | Fake Access Points | Creates **rogue access points** for testing **man-in-the-middle (MITM) attacks** or Wi-Fi security. |

---
10.10.10.0/24
10.10.11.0/24
10.10.12.0/24
192.168.0.0/16
The IP addresses provided are RFC 1918 addresses.
---

# Active vs. Passive Scanning  

| **Feature**         | **Active Scanning** | **Passive Scanning** |
|---------------------|--------------------|----------------------|
| **Definition** | Actively probes the target system for vulnerabilities. | Monitors network traffic without direct interaction. |
| **Methodology** | Sends requests to the system and analyzes responses. | Captures and analyzes traffic without sending probes. |
| **Examples** | Port scanning, vulnerability scanning, network mapping. | Network sniffing, monitoring logs, passive fingerprinting. |
| **Tools Used** | Nmap, Nessus, OpenVAS, Qualys. | Wireshark, tcpdump, Zeek (Bro). |
| **Impact on Target** | Can be detected and blocked by IDS/IPS or firewalls. | Stealthy and harder to detect. |
| **Risk Level** | Higher—may trigger alerts or cause disruptions. | Lower—does not generate direct traffic. |
| **Use Cases** | Penetration testing, vulnerability assessments, compliance audits. | Threat intelligence gathering, incident response, reconnaissance. |
| **Detection Likelihood** | Easier to detect (logs, alerts, firewall triggers). | Harder to detect (observes existing traffic). |

---

## Components of Security Content Automation Protocol (SCAP)
- The Common Vulnerabilities and Exposures (CVE) database provides a consistent reference for identifying security vulnerabilities. 
- The Open Vulnerability and Assessment Language (OVAL) is used to describe the security condition of a system. 
- The Extensible Configuration Checklist Description Format (XCCDF) is used to create security checklists in a standardized fashion. 
- The Script Check Engine (SCE) is designed to make scripts interoperable with security policy definitions.
- Common Platform Enumeration (CPE) provides a consistent way to refer to operating systems and other system components
---

# Security Scanning Types Comparison

| **Scan Type**             | **Definition**  | **Purpose**  | **Example Tools**  | **CISSP Domain** |
|---------------------------|----------------|--------------|--------------------|------------------|
| **Authenticated Scan**     | Uses valid credentials to scan internal systems. | Identifies **deep system vulnerabilities**. | Nessus, Qualys, OpenVAS | Domain 6, 7 |
| **Web Application Scan**   | Scans web apps for **XSS, SQL Injection, and authentication issues**. | Secures websites & APIs. | Burp Suite, OWASP ZAP, Acunetix | Domain 8, 6 |
| **Unauthenticated Scan**   | Simulates an **external attacker** scanning a system **without login credentials**. | Finds **publicly exposed vulnerabilities**. | Nmap, Nessus, OpenVAS | Domain 6, 7 |
| **Port Scan**              | Identifies **open, closed, or filtered ports** on a system. | Checks for **running services and misconfigurations**. | Nmap, Angry IP Scanner | Domain 4, 6 |

## **Key Takeaways**
- **Authenticated scans** give deep insights using valid login credentials.
- **Unauthenticated scans** mimic external attacks to find exposed vulnerabilities.
- **Web application scans** focus on web-based threats like **XSS, SQL Injection**.
- **Port scans** help discover **open services** and **network security posture**.

---

**Requirement Traceability Matrices**

Employing the RTM as a dynamic, iterative tool that adjusts to changing requirements over time is the most significant aspect. This approach ensures that the RTM stays relevant and useful throughout the software development lifecycle, capturing changes in requirements, project tasks, and deliverable documents, as well as adapting to evolving security landscapes. This continuous adaptation and tracking of requirements are key to avoiding overlooked elements and mitigating potential vulnerabilities. The incorrect answers: Updating the RTM to reflect the requirements of every new software version is an important practice, but it's not the most significant aspect. This practice ensures that the new requirements are documented, but it doesn't necessarily ensure that the RTM evolves with changing project needs or that the implementation of these requirements is tracked effectively. Having the RTM encompass all software requirements, including project tasks and deliverable documents, is crucial for comprehensive project management. But the breadth of information included in the RTM is less significant than how this information is used and updated over time, particularly as the requirements and priorities of a project may change. Including specific security requirements in the RTM from the start is a best practice, as it embeds security into the software development process. Nevertheless, while this is important, it does not address the need for these requirements to be adaptable over time in response to changing threats and project objectives.

---