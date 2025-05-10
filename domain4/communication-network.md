# 🧵 Cat 5 / Cat 6 Twisted Pair Cables

## 🧠 What is a Twisted Pair?

A **twisted pair** cable consists of pairs of insulated copper wires twisted together to reduce electromagnetic interference (EMI) and crosstalk between adjacent wires.

---

## 🧪 Categories: Cat 5 vs Cat 6

| Feature              | Cat 5 / Cat 5e                | Cat 6                       |
|----------------------|-------------------------------|-----------------------------|
| 📶 Frequency Range   | Up to 100 MHz                 | Up to 250 MHz               |
| 🚀 Max Data Speed    | 100 Mbps (Cat 5) <br> 1 Gbps (Cat 5e) | 1 Gbps (up to 100m) <br> 10 Gbps (up to 55m) |
| 🔌 Cable Type        | Unshielded Twisted Pair (UTP) | Usually UTP, sometimes shielded (STP) |
| 🔧 Internal Separator| No                            | Yes (cross-separator reduces crosstalk) |
| 🧯 Interference Resistance | Good                   | Better (less crosstalk and EMI) |
| 💰 Cost              | Cheaper                       | Slightly more expensive     |

---

## 🛠️ Use Cases

- **Cat 5**: Obsolete; not used in new installations.
- **Cat 5e**: Common for home networks, supports Gigabit Ethernet.
- **Cat 6**: Preferred for office environments and new installations with higher data rate needs (Gigabit or 10-Gigabit LAN).

---

## 🧷 Summary

- **Cat 5e** is the enhanced version of Cat 5, supporting up to 1 Gbps.
- **Cat 6** provides **better performance**, especially over short distances, and is more **future-proof** for faster networks.
- Both use **RJ45 connectors** and support **Ethernet, Fast Ethernet, and Gigabit Ethernet**.

---

# 🛡️ Types of NAC (Network Access Control) Systems

Network Access Control (NAC) systems help enforce security policies on devices seeking access to a network. They inspect endpoints and grant, deny, or restrict access based on compliance.

---

# 🛡️ Deep Dive into NAC (Network Access Control)

## 📘 What is NAC?

**Network Access Control (NAC)** is a security solution that manages and controls access to a network based on predefined policies. NAC ensures that only authenticated, compliant, and trusted devices and users can connect to a network.

---

## 🎯 Objectives of NAC

- 🔐 Enforce **identity and device verification**.
- ⚙️ Control **what devices/users can access**.
- 🧪 Evaluate endpoint **compliance posture** (e.g., antivirus, OS version).
- 🚫 Quarantine or restrict **non-compliant** systems.
- 📊 Provide **visibility** into connected devices.

---

## 🧱 Core Components of NAC

| Component              | Function                                      |
|------------------------|-----------------------------------------------|
| **Authentication**     | Verifies user or device identity (e.g., RADIUS, 802.1X). |
| **Policy Engine**      | Determines access based on defined rules.     |
| **Posture Assessment** | Checks device security status (e.g., antivirus up to date). |
| **Enforcement Point**  | Switch, router, or firewall that grants/blocks access. |
| **Remediation**        | Redirects non-compliant systems to a remediation network. |

---

## 🛠️ NAC Workflow

1. **Device attempts to connect** to the network.
2. NAC performs **identity/authentication** check.
3. **Posture assessment** is conducted (optional).
4. Access is either:
   - ✅ **Granted** (full or limited),
   - 🔒 **Denied**, or
   - 🔁 **Redirected** for **remediation**.
5. Continuous **monitoring** and **enforcement** post-admission.

---

## 🧩 Types of NAC

### 1. **In-Band (Inline) NAC**
- NAC device is in the **data path**.
- Monitors and enforces traffic in real time.
- Example: Forescout CounterACT.

### 2. **Out-of-Band NAC**
- NAC is **not inline**; uses control protocols (RADIUS, SNMP) to enforce policy.
- Common in **802.1X-based** architectures.
- Example: Cisco ISE, Aruba ClearPass.

---

## 🕵️ Pre-admission vs Post-admission NAC

| Type             | Description                           |
|------------------|---------------------------------------|
| **Pre-admission**| Checks device compliance **before** granting access. |
| **Post-admission**| Monitors behavior **after** access is granted.        |

---

## 🔐 Common Authentication Protocols Used

- **802.1X**: Port-based access control.
- **RADIUS**: Centralized authentication, authorization, accounting.
- **LDAP**: Directory-based user verification.
- **TACACS+**: Cisco’s alternative to RADIUS.

---

## 💡 Use Cases

- **Guest networking** with access restrictions.
- **BYOD** (Bring Your Own Device) control.
- **Contractor access** limitation.
- **IoT device** segmentation.
- **Endpoint compliance** enforcement.

---

## 🧪 Posture Checks Typically Include:

- OS type and version.
- Antivirus installation and update status.
- Patch level.
- Device type (e.g., mobile, laptop, IoT).
- Firewall status.

---

## 🛠️ Popular NAC Solutions

| Vendor         | Solution Name         |
|----------------|------------------------|
| Cisco          | Identity Services Engine (ISE) |
| Fortinet       | FortiNAC               |
| HPE/Aruba      | ClearPass              |
| Forescout      | CounterACT             |
| Microsoft      | Intune (modern replacement for NAP) |
| Sophos         | NAC Advanced           |

---

## ✅ Benefits of NAC

- 🚧 Prevent unauthorized access.
- 🔍 Increase network visibility.
- 🔄 Automate access control and compliance enforcement.
- 📉 Reduce risk of malware and data breaches.

---

## ⚠️ Challenges

- 🔧 Complex deployment and configuration.
- 📡 Requires integration with existing infrastructure.
- 🖥️ Performance overhead on large-scale networks.
- 🧠 User/device behavior learning curve.

---

## 🧠 Summary

**NAC** is a critical component of modern enterprise security. It provides granular control over **who and what can connect** to a network, enforces **security policies**, and ensures **endpoint compliance**. With the rise of **BYOD, IoT, and hybrid work**, NAC has become essential for **zero-trust architecture**.

---

## 🧠 Examples of NAC Solutions

| Vendor         | NAC Solution Name         |
|----------------|---------------------------|
| Cisco          | Cisco Identity Services Engine (ISE) |
| Fortinet       | FortiNAC                  |
| Aruba (HPE)    | ClearPass                 |
| Forescout      | CounterACT                |
| Microsoft      | NAP (obsolete), Intune (modern alternative) |

---

## ✅ Summary

| Type            | Description                            | Deployment Stage |
|-----------------|----------------------------------------|------------------|
| In-Band NAC     | Inline traffic inspection              | Pre/Post         |
| Out-of-Band NAC | Uses external enforcement              | Pre/Post         |
| Pre-admission   | Endpoint validated before access       | Pre              |
| Post-admission  | Endpoint monitored after access        | Post             |

---