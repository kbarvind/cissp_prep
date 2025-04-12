
- **Coupling** is a description of the level of interaction between objects. 
- **Cohesion** is the strength of the relationship between the purposes of methods within the same class. When you are developing an object-oriented model, it is desirable to have high cohesion and low
coupling.

---

- **Cross-site request forgery (XSRF or CSRF)** attacks exploit the trust that sites have in a user’s browser by attempting to force the submission of authenticated requests to thirdparty sites. 
- **Session hijacking** attacks attempt to steal previously authenticated sessions but do not force the browser to submit requests. 
- **SQL injection** directly attacks a database through a web application. 
- **Cross-site scripting** uses reflected input to trick a user’s browser into executing untrusted code from a trusted site.

---

| **Term**       | **Definition**                                                                                   | **CISSP Context / Relevance**                                                                 |
|----------------|--------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| **Inference**  | The process of deducing sensitive information from non-sensitive data using logic and correlation. | Related to data leakage risks in **Asset Security**; users may infer secrets without direct access. |
| **Polymorphic**| Refers to code that can change its form while keeping the same function, often used by malware.   | Seen in **malware evasion techniques** (e.g., polymorphic viruses) under **Security Operations (Domain 7)**. |
| **Aggregate**  | Combining multiple pieces of lower-classified data to derive higher-level sensitive information.  | A data exposure method discussed in **Asset Security**; often controlled via query restrictions. |
| **Modular**    | A design approach that separates a system into independent, interchangeable components.           | Used in **secure software development** (Domain 8); helps isolate functions and limit impact. |

-----