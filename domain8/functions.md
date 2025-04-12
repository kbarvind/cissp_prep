# 📚 CISSP Cheat Sheet: Inference vs Aggregation

## 🔍 Overview

Understanding the difference between **Inference** and **Aggregation** is essential for preventing unauthorized data disclosure through indirect methods. These concepts are part of **CISSP Domain 2: Asset Security**.

---

## 🧠 Key Comparison

| **Concept**       | **Description**                                                           | **Example Scenario**                                                | **Key Security Control**                                               |
|------------------|---------------------------------------------------------------------------|---------------------------------------------------------------------|------------------------------------------------------------------------|
| **Aggregation**  | Combining non-sensitive data to reveal sensitive info                     | Using `SUM(salary)` across a department to guess an executive's pay | Aggregation control, query restriction, cell suppression              |
| **Inference**    | Deduction of sensitive information using logical reasoning from available data | Inferring illness based on repeated doctor visits in logs           | Inference detection, noise, data masking, query analysis              |

---

## 🔄 Simplified View

| **Term**         | **What is it?**                          | **How is it done?**                    |
|------------------|------------------------------------------|----------------------------------------|
| **Aggregation**  | Unauthorized insight via data combination | Running summary (e.g., AVG, COUNT)     |
| **Inference**    | Unauthorized insight via logical deduction| Observing patterns, metadata, behavior |

---

## ✅ CISSP Question Pattern Example

> An attacker is combining multiple allowed data queries to learn the salary of a senior executive by summing all other salaries.  
> **What is the attack type?**

**Answer:** `Aggregation`

---

## 🛡️ Defense Mechanisms

| **Technique**             | **Purpose**                                      |
|---------------------------|--------------------------------------------------|
| **Cell suppression**       | Hides sensitive values in query results          |
| **Query restriction**      | Prevents queries that return too few records     |
| **Noise/Perturbation**     | Adds randomness to obscure sensitive data        |
| **Data masking / Views**   | Restricts what is visible at application level   |
| **Audit logs**             | Monitor and review user queries                  |

---

## 📌 Tip:
> Aggregation = Function misuse  
> Inference = Logical deduction  
Both lead to **data leakage**, even when users are within their access levels!

