# Commonly Used Ports in Windows and Linux (CISSP Perspective)

| **Port**  | **Protocol** | **Service** | **OS** | **Usage** |
|-----------|------------|------------|--------|-----------|
| **20**   | TCP | FTP (Data Transfer) | Linux/Windows | Used in active mode FTP connections |
| **21**   | TCP | FTP (Control) | Linux/Windows | File transfer service |
| **22**   | TCP | SSH | Linux | Secure remote access |
| **23**   | TCP | Telnet | Linux/Windows | Unencrypted remote access (Legacy, insecure) |
| **25**   | TCP | SMTP | Linux/Windows | Email sending (mail servers) |
| **53**   | TCP/UDP | DNS | Linux/Windows | Domain Name System resolution |
| **67/68** | UDP | DHCP | Linux/Windows | Assigns dynamic IP addresses |
| **69**   | UDP | TFTP | Linux | Trivial File Transfer (PXE boot, firmware updates) |
| **80**   | TCP | HTTP | Linux/Windows | Web browsing (web servers) |
| **88**   | TCP/UDP | Kerberos | Windows | Authentication service (Active Directory) |
| **110**  | TCP | POP3 | Linux/Windows | Email retrieval |
| **123**  | UDP | NTP | Linux/Windows | Network Time Protocol (time synchronization) |
| **135**  | TCP/UDP | RPC | Windows | Remote Procedure Call (Windows DCOM services) |
| **137-139** | TCP/UDP | NetBIOS | Windows | File sharing (SMB over NetBIOS) |
| **143**  | TCP | IMAP | Linux/Windows | Email retrieval (modern alternative to POP3) |
| **161/162** | UDP | SNMP | Linux/Windows | Network monitoring and management |
| **389**  | TCP/UDP | LDAP | Linux/Windows | Directory services (Active Directory, OpenLDAP) |
| **443**  | TCP | HTTPS | Linux/Windows | Secure web browsing |
| **445**  | TCP | SMB | Windows | File sharing (Direct SMB over TCP) |
| **465**  | TCP | SMTPS | Linux/Windows | Secure SMTP (email sending) |
| **514**  | UDP | Syslog | Linux | System logging |
| **636**  | TCP | LDAPS | Linux/Windows | Secure LDAP (Active Directory, Linux directory services) |
| **989/990** | TCP | FTPS | Linux/Windows | Secure FTP |
| **993**  | TCP | IMAPS | Linux/Windows | Secure IMAP (email retrieval) |
| **995**  | TCP | POP3S | Linux/Windows | Secure POP3 (email retrieval) |
| **1433** | TCP | Microsoft SQL Server | Windows | Database service |
| **1521** | TCP | Oracle Database | Linux/Windows | Oracle database connectivity |
| **3306** | TCP | MySQL | Linux | Open-source database service |
| **3389** | TCP | RDP | Windows | Remote Desktop Protocol |
| **5900** | TCP | VNC | Linux | Remote desktop access |
| **8080** | TCP | HTTP Alternate | Linux/Windows | Web proxy, application servers |

## Why These Ports Matter for CISSP?
1. **Security Risks** – Unsecured services like **Telnet (23)**, **FTP (21)**, and **SMB (445)** can be exploited.
2. **Firewall Configurations** – Security controls rely on **allowing/blocking ports**.
3. **Intrusion Detection** – Port scanning is a common **reconnaissance technique**.
4. **Incident Response** – Identifying suspicious traffic on ports like **445 (SMB - WannaCry attack)** or **3389 (RDP - brute force attacks)**.