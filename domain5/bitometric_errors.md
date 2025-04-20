# 👁️‍🗨️ Biometric Error Types

Biometric systems can produce various errors during enrollment and authentication. Here's a summary of the most common ones:

---

## 🔐 1. False Acceptance Rate (FAR)

- **Definition**: The rate at which an unauthorized user is incorrectly accepted by the system.
- **Risk Type**: **Security risk**
- **Example**: The system allows access to someone else's fingerprint.

---

## ❌ 2. False Rejection Rate (FRR)

- **Definition**: The rate at which a legitimate, authorized user is incorrectly rejected.
- **Risk Type**: **Usability risk**
- **Example**: Your voice isn’t recognized due to a sore throat.

---

## ⚖️ 3. Equal Error Rate (EER)

- **Definition**: The point where **FAR = FRR**.
- **Use**: Used as a benchmark for biometric system accuracy — the **lower the EER, the better**.

---

## 🧾 4. Failure to Enroll (FTE)

- **Definition**: The system cannot register a biometric sample for the user.
- **Cause**: Poor biometric traits (e.g., worn fingerprints, damaged iris).
- **Impact**: User cannot use the system at all.

---

## 📷 5. Failure to Capture (FTC)

- **Definition**: The system fails to capture a usable biometric sample during authentication.
- **Cause**: Dirty sensors, bad lighting, or user positioning.
- **Impact**: Authentication process is interrupted or fails.

---

## 📊 Summary Table

| Error Type         | Description                                                 | Risk Type       | Example Scenario                                      |
|--------------------|-------------------------------------------------------------|------------------|-------------------------------------------------------|
| **FAR**            | Unauthorized user accepted                                  | Security Risk    | Attacker gains access with similar fingerprint        |
| **FRR**            | Authorized user rejected                                     | Usability Risk   | Legit user denied due to poor scan                    |
| **EER**            | Point where FAR = FRR                                       | Accuracy Metric  | Used to compare system performance                    |
| **FTE**            | System can't register user's biometric                      | Usability Risk   | Fingerprint unreadable during setup                  |
| **FTC**            | System can't capture biometric at scan time                 | Technical Issue  | Finger not placed properly or sensor malfunction     |