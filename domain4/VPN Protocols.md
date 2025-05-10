# 🔐 Common VPN Protocols

This document lists commonly used VPN protocols, including their key features, encryption methods, and typical use cases.

---

## ✅ VPN Protocol Comparison Table

| Protocol        | Transport Layer          | Encryption        | Notes                                                                 |
|-----------------|--------------------------|-------------------|-----------------------------------------------------------------------|
| **IPsec (IKEv1/IKEv2)** | Network Layer (IP)        | AES, 3DES          | Used for site-to-site and remote access VPNs. Secure and efficient.   |
| **OpenVPN**     | User Space (TCP/UDP)     | AES, ChaCha20     | Open source and highly configurable. Good for bypassing firewalls.    |
| **WireGuard**   | Network Layer (UDP)      | ChaCha20          | Modern, fast, lightweight, with a simpler codebase.                   |
| **SSL VPN**     | Application Layer (HTTPS)| TLS (AES, etc.)   | Enterprise remote access via browser or client. Firewall-friendly.    |
| **L2TP/IPsec**  | Layer 2 + Network Layer  | AES, 3DES         | L2TP handles tunneling; IPsec provides encryption. Legacy support.    |
| **PPTP**        | Tunneling (Layer 2)      | MPPE (128-bit)    | Fast but outdated and insecure. **Not recommended.**                  |
| **SSTP**        | SSL over TCP (443)       | TLS (AES, etc.)   | Developed by Microsoft. Native to Windows and firewall-friendly.      |

---

## 📝 Summary: Security, Speed, and Use Case

| Protocol       | Security     | Speed       | Platform Support         | Recommended Use                           |
|----------------|--------------|-------------|--------------------------|-------------------------------------------|
| **WireGuard**  | ⭐⭐⭐⭐⭐        | ⭐⭐⭐⭐⭐       | Linux, iOS, Android, Windows | Modern and fast VPN (recommended)        |
| **OpenVPN**    | ⭐⭐⭐⭐         | ⭐⭐⭐         | Cross-platform           | Secure, widely adopted                    |
| **IPsec/IKEv2**| ⭐⭐⭐⭐         | ⭐⭐⭐⭐        | Built-in on many OSes    | Site-to-site, mobile VPNs                 |
| **SSL VPN**    | ⭐⭐⭐⭐         | ⭐⭐⭐         | Browser/client-based     | Remote access, firewall-friendly          |
| **L2TP/IPsec** | ⭐⭐⭐          | ⭐⭐          | Legacy support           | Use only when IPsec/IKEv2 isn't available |
| **SSTP**       | ⭐⭐⭐          | ⭐⭐          | Windows native           | For Windows clients behind firewalls      |
| **PPTP**       | ❌ (insecure) | ⭐⭐⭐⭐        | Legacy platforms         | Avoid – deprecated                        |

---

## 🔒 Key Takeaways

- **Best Security & Speed:** WireGuard
- **Most Versatile:** OpenVPN
- **Best for Enterprises:** SSL VPN or IPsec/IKEv2
- **Avoid:** PPTP due to weak security