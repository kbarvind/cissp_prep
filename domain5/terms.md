# 🔐 SAML vs SPML — Key Differences

| Feature               | **SAML** (Security Assertion Markup Language)         | **SPML** (Service Provisioning Markup Language)           |
|-----------------------|--------------------------------------------------------|------------------------------------------------------------|
| **Purpose**           | Authentication and authorization (SSO)                 | User provisioning and lifecycle management                 |
| **Use Case**          | Single Sign-On (SSO) between IdP and service providers | Creating, updating, and deleting user accounts             |
| **Who Uses It**       | Web apps, federated identity providers                 | Identity management systems (IdM/IdAM)                     |
| **Focus**             | **Access control** — verifying identity                | **Account management** — controlling account lifecycle     |
| **Typical Scenario**  | Logging into Salesforce via corporate login            | HR system creates a user account in Active Directory       |
| **Example Assertion** | “User is authenticated and belongs to HR.”            | “Create a new user with role: HR Manager.”                 |
| **Protocol Base**     | XML-based assertions                                   | XML-based provisioning commands                            |
| **Industry Support**  | Widely adopted (e.g., Okta, Azure AD, SSO systems)     | Less widely used (often replaced by SCIM)                 |

---

# 🔐 Pass-the-Hash vs Salt Recovery Attack — Key Differences Summary

| Feature                  | **Pass-the-Hash (PtH)**                          | **Salt Recovery Attack**                              |
|--------------------------|--------------------------------------------------|--------------------------------------------------------|
| **Attack Type**          | Authentication bypass                           | Hash cracking aid                                     |
| **Target**               | Hash in memory or disk (usually NTLM)           | Stored password hashes + salts                        |
| **Goal**                 | Use hash directly to authenticate                | Guess/recover salt to simplify hash cracking          |
| **Requires Cracking?**   | ❌ No                                             | ✅ Yes                                                 |
| **Common Tool**          | Mimikatz, Metasploit                             | Hashcat, John the Ripper                              |
| **Environment Targeted** | Windows environments (NTLM, SMB)                 | Systems using salted password hashes                  |
| **Defense**              | Use Kerberos, Credential Guard, limit privileges| Use strong, unique salts and slow hashing algorithms  |

---

# 🔐 Cross-Site Request Forgery (CSRF)

Cross-Site Request Forgery (CSRF) is a type of web security vulnerability that allows an attacker to trick a user into performing actions that they did not intend to perform. This is done by exploiting the trust that a web application has in the user's browser.

## Key Characteristics of CSRF

- **Attack Vector**: The attacker crafts a malicious request and tricks the user into executing it, often by embedding the request in a link or a hidden form on a third-party website.
- **Impact**: If successful, the attacker can perform actions on behalf of the user, such as changing account settings, making transactions, or any other action the user is authorized to perform.
- **Target**: CSRF targets state-changing requests, not data theft, as the attacker cannot see the response to the forged request.

## Defense Mechanisms

1. **CSRF Tokens**: Implement anti-CSRF tokens in forms and validate them on the server side to ensure that the request is legitimate.
2. **SameSite Cookies**: Use the SameSite attribute in cookies to prevent them from being sent with cross-site requests.
3. **User Interaction**: Require user interaction, such as re-authentication or CAPTCHA, for critical actions.

## Example Scenario

A user is logged into their bank account. An attacker sends them a link to a malicious website that contains a hidden form that, when submitted, transfers money from the user's account to the attacker's account. If the user visits the malicious site while logged in, the form is submitted automatically, and the transaction is completed without the user's knowledge.

---


## 🔐 Dynamic Knowledge-Based Authentication (KBA)

Dynamic Knowledge-Based Authentication (KBA) is a method of identity verification that uses questions generated in real-time based on the user's personal information. Unlike static KBA, which relies on pre-set questions and answers, dynamic KBA pulls information from various data sources to create questions that are unique to the user and difficult for an imposter to answer.

### Key Characteristics of Dynamic KBA

- **Real-Time Question Generation**: Questions are generated on-the-fly using data from credit reports, public records, or other databases.
- **Enhanced Security**: By using unpredictable questions, dynamic KBA reduces the risk of unauthorized access compared to static KBA.
- **User-Specific**: Questions are tailored to the individual, making it challenging for attackers to guess or find answers.

### Example Scenario

During an online banking login, the system asks the user to verify their identity by answering questions about recent transactions or addresses associated with their credit history.




## 🔐 Out-of-Band Identity Spoofing

Out-of-Band Identity Spoofing is a type of attack where an attacker intercepts or manipulates communication channels that are separate from the primary communication path. This method is often used to bypass security measures that rely on multi-factor authentication (MFA) or other out-of-band verification processes.

### Key Characteristics of Out-of-Band Identity Spoofing

- **Separate Communication Channel**: The attack targets channels like SMS, email, or phone calls used for verification.
- **Exploitation of Trust**: Attackers exploit the trust users place in these secondary channels to gain unauthorized access.
- **Common Targets**: Systems using SMS-based OTPs (One-Time Passwords) or phone call verifications are particularly vulnerable.

### Example Scenario

An attacker intercepts an SMS containing a one-time password sent to a user's phone and uses it to gain access to the user's account.



## 🔐 Type 3 Authentication

Type 3 Authentication, also known as "Something You Are," refers to biometric authentication methods that rely on unique physical characteristics of an individual. This type of authentication is considered highly secure because it is based on inherent traits that are difficult to replicate or steal.

### Key Characteristics of Type 3 Authentication

- **Biometric Traits**: Includes fingerprints, facial recognition, iris scans, voice recognition, and other physiological or behavioral characteristics.
- **High Security**: Provides strong security due to the uniqueness and difficulty of duplicating biometric data.
- **User Convenience**: Often more convenient for users as it eliminates the need to remember passwords or carry tokens.

### Example Scenario

A smartphone uses facial recognition to unlock the device, ensuring that only the authorized user can access its contents.


---

