
# 📘 Design Approaches in Secure Software Development

### **Design Approaches in Secure Software Development**

| **Approach**        | **Description**                                                                                     | **CISSP Relevance**                                                      |
|---------------------|-----------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------|
| **Modular Design**  | Divides a system into independent, interchangeable modules, improving maintainability and reusability. | Promotes separation of concerns, making it easier to secure individual modules. |
| **Layered Design**  | Divides a system into layers (e.g., presentation, business logic, data access) to isolate functionality and promote security. | **Defense in depth**; ensures that layers are independently secure.     |
| **Component-Based Development (CBD)** | Focuses on developing reusable, independent components that can be plugged into different systems. | Reusability increases security by ensuring stable, tested components.   |
| **Service-Oriented Architecture (SOA)** | Breaks down applications into smaller services, which communicate through well-defined interfaces. | Promotes security by isolating services, simplifying access controls, and allowing for isolated security measures per service. |
| **Microservices**   | A more granular version of SOA, where systems are broken down into small, independently deployable services. | Enhances security by minimizing attack surfaces, as each service can be secured independently. |
| **Object-Oriented Design (OOD)** | Uses objects (data structures) and methods to create systems that encapsulate behavior and data together. | Reduces risk by encouraging encapsulation and data hiding, which are security best practices. |
| **Client-Server Model** | A network architecture where one machine (server) provides services to another machine (client). | Centralized security management is possible, allowing better control over sensitive data. |
| **Event-Driven Architecture (EDA)** | A system where components communicate primarily through events and responses. | Provides better control over security events and helps manage asynchronous operations securely. |
| **Rule-Based Design** | Defines explicit rules for how software should behave under various conditions, often using decision tables or other rule-based mechanisms. | Adds clarity to security policies by enforcing specific rules for processing data. |

---

### **Approach Benefits:**
- **Modular** and **Layered** designs help isolate **security vulnerabilities** to specific components or layers.
- **Component-Based** and **Service-Oriented** approaches encourage **reuse of proven, secure components**.
- **Microservices** promote **small, isolated environments**, reducing the scope of potential attacks.
- **Object-Oriented Design** ensures **encapsulation** and **information hiding**, which enhances security.

---

### **Security Benefits of These Approaches:**
- **Defense in Depth**: Layered and modular designs enhance defense strategies by making it harder for attackers to break through all layers.
- **Granular Control**: Microservices, SOA, and component-based approaches allow **independent security enforcement** at each level or service.
- **Reusability**: Using tested, secure components reduces the likelihood of introducing vulnerabilities.

---


# 🏗️ Software Capability Maturity Model (SW-CMM) – Phases

| **Level** | **Name**             | **Description**                                                                                  | **Key Process Areas**                                      |
|-----------|----------------------|--------------------------------------------------------------------------------------------------|-------------------------------------------------------------|
| **Level 1** | Initial              | Process is ad hoc and chaotic. Success depends on individual efforts rather than on repeatable processes. | None formally defined                                       |
| **Level 2** | Repeatable           | Basic project management processes are established. Allows for repeatable success on similar projects. | - Requirements Management  <br> - Project Planning <br> - Project Monitoring and Control <br> - Supplier Agreement Management <br> - Configuration Management |
| **Level 3** | Defined              | Processes are documented, standardized, and integrated into a standard software process across the organization. | - Organizational Process Focus <br> - Training Program <br> - Integrated Software Management <br> - Product Engineering |
| **Level 4** | Managed              | Process and product quality are measured. Quantitative goals are set and measured.               | - Quantitative Process Management <br> - Software Quality Management |
| **Level 5** | Optimizing           | Focus on continuous process improvement through feedback and innovation.                        | - Defect Prevention <br> - Technology Change Management <br> - Process Change Management |