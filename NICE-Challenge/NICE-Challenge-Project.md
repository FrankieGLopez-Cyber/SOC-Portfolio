# NICE Challenge – Volatile Vulnerabilities (NG)

**Submission ID:** 64406  
**Challenge ID:** 123  
**Date:** February 20, 2022  
**Duration:** 1 hr 19 min  
**Result:** ✅ **Full Check Pass (8/8)**

 **Click here to view the full NICE Challenge PDF report**](NICE-Challenge/FrankieLopez_NCPReport1Challenge.pdf)

---

## 🧠 Scenario
A security gap was identified where users in the HR and Accounting departments could access each other’s applications, creating a **confidentiality and internal access control risk**.

**Objective:**  
Enforce **role-based application access** to ensure:
- HR users can only run the HR application  
- Accounting users can only run the Accounting application  

---

## ⚙️ Actions Taken
- Created and linked a **domain-level GPO (DasApp Policy)**  
- Enabled the **Application Identity Service** to support AppLocker  
- Configured **AppLocker Executable Rules** to control permitted applications  
- Generated **Default Allowed Rules** to maintain OS stability  
- Implemented **Explicit Deny Rules** to:
  - Block HR users from launching the Accounting app  
  - Block Accounting users from launching the HR app  

---

## 🧰 Tools & Technologies
- Windows Server / Active Directory  
- Group Policy Management Console (GPMC)  
- AppLocker (Executable Policy Enforcement)  
- Security Policy Editor  
- AD Users, Groups & OU Management  

---

## 📊 Outcome
| Result | Description |
|--------|-------------|
| ✅ | All 8 validation checks passed |
| 🔐 | Department application access successfully isolated |
| 🚫 | Cross-department execution attempts blocked |
| 📏 | System now enforces **Least Privilege & Separation of Duties** |

---

## 🔥 Security Impact
This configuration:
- **Eliminates unauthorized internal data access**
- Protects **sensitive HR and financial information**
- Ensures **policy-based enforcement**, not trust-based access
- Demonstrates **Zero Trust** and **Role-Based Access Control (RBAC)** principles

Supports compliance frameworks:
- **NIST 800-53 (AC-1, AC-3)**
- **SOX** (Internal Access Governance)
- **HIPAA Privacy Controls**

---

## 🧩 NICE Framework Alignment

| Category | Code | Demonstrated Capability |
|---------|------|------------------------|
| **Task** | T0123 | Implement system/application cybersecurity controls |
| **Knowledge** | K0060 | Operating system security configuration |
| **Knowledge** | K0049 | Enterprise security boundary/segmentation |
| **Skill** | S0031 | Apply system access control configurations |
| **Skill** | S0147 | Assess effectiveness of applied controls |

---

## 🏁 Summary
This challenge demonstrates the ability to **design and enforce application access controls** using Active Directory and AppLocker to prevent improper internal data access.  
It reflects real-world competencies required in:
- **SOC Analyst**
- **IAM Analyst**
- **Security Administrator**

Looking back, a key takeaway from this challenge was how sensitive AppLocker configurations are to scope and inheritance.
Ensuring that each department had clearly defined allow/deny rules reinforced the importance of validating policy behavior rather than assuming access is segmented by default.
Even though this lab was done some time ago, the concepts stuck with me — particularly how role-based controls must be tested from both perspectives (HR → Accounting and vice versa) to confirm that least privilege is truly enforced.

**Core Strength Demonstrated:** Practical implementation of **Least Privilege** and **Zero Trust** policy enforcement in a Windows enterprise environment.
