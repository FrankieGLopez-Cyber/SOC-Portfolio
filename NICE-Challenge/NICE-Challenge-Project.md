# NICE Challenge – Volatile Vulnerabilities [NG]
**Submission ID:** 64406  
**Challenge ID:** 123  
**Date:** February 20, 2022  
**Duration:** 1 hr 19 min  
**Result:** ✅ Full Check Pass (8/8)

[**Click here to view the full NICE Challenge PDF report**][(NICE-Challenge/FrankieLopez_NCPReport1Challenge.pdf)](https://github.com/FrankieGLopez-Cyber/SOC-Portfolio/blob/main/NICE-Challenge/FrankieLopez_NCPReport1Challenge.pdf)
 
---

### 🧠 Scenario
A vulnerability was discovered within the organization’s **HR and Accounting applications**, which allowed cross-departmental access to sensitive data.  
My objective was to design and enforce access controls preventing unauthorized use of either application by users from the opposite department.

---

### ⚙️ Actions Taken
1. Created and linked a **GPO (DasApp Policy)** at the domain level.  
2. Enabled **Application Identity Service** within the policy.  
3. Configured **AppLocker Executable Enforcement**.  
4. Generated three **Default AppLocker Rules**.  
5. Used AppLocker to:
   - Deny HR users from accessing the Accounting app.  
   - Deny Accounting users from accessing the HR app.

---

### 🧰 Tools & Technologies
- **Windows Server / Active Directory**
- **Group Policy Management Console (GPMC)**
- **AppLocker (Executable Rules)**
- **Security Policy Editor**
- **User/Group Permission Management**

---

### 📊 Outcome
- All 8 validation checks passed successfully.  
- HR and Accounting apps were properly isolated via AppLocker enforcement.  
- System configuration fully met the scenario’s confidentiality and access control requirements.

---

### 🧩 NICE Framework Alignment
**Work Role:** Systems Security Analyst  
**Task:** T0123 – Implement specific cybersecurity countermeasures for systems and/or applications.  

**Knowledge, Skills, and Abilities Demonstrated:**
- K0004 – Cybersecurity and privacy principles  
- K0049 – IT security methods (firewalls, encryption, zones)  
- K0060 – Operating system security configuration  
- K0276 – Security management concepts  
- K0297 – Countermeasure design  
- S0001 – Vulnerability recognition and mitigation  
- S0031 – System access control implementation  
- S0147 – Assessment of security controls

---

### 🧩 Related Knowledge Units
- Cybersecurity Foundations  
- Operating Systems Hardening  
- Windows System Administration  

---

🔗 [[Official NICE Challenge](https://github.com/FrankieGLopez-Cyber/SOC-Portfolio/blob/main/NICE-Challenge/FrankieLopez_NCPReport1Challenge.pdf)







NICE Challenge – Volatile Vulnerabilities (NG)

Submission ID: 64406
Challenge ID: 123
Date: Feb 20, 2022
Result: ✅ Full Pass (8/8 Validations)
Duration: 1 hr 19 min

📄 View Full Challenge Report

🧠 Scenario

The organization discovered that HR and Accounting applications lacked proper access segmentation — allowing users in one department to open and interact with applications intended for the other. This posed a data confidentiality and internal access control risk.

Objective

Restrict application access so:

HR users can only run the HR application

Accounting users can only run the Accounting application

⚙️ Actions Taken
Control Implemented	Purpose	Tool Used
Created GPO (DasApp Policy)	Centralized enforcement of access policy	Group Policy Mgmt Console
Enabled Application Identity Service	Supports AppLocker execution rules	Services.msc / GPMC
Configured AppLocker Executable Rules	Controlled which users can run which apps	Local/Domain Policy
Generated Default Allowed Rules	Ensured OS stability while enforcing restrictions	AppLocker
Applied Explicit Deny Rules	Prevent cross-department app execution	AppLocker + AD Group Membership
🛡️ Security Purpose

This configuration enforces least privilege and zero trust segmentation between internal user roles.

🧰 Tools & Technologies

Windows Server / Active Directory

Group Policy Management Console (GPMC)

AppLocker Policy Enforcement

Security Policy Editor

Organizational Unit / Group Permission Management

📊 Outcome

✅ All 8 validation checks passed
🔐 HR and Accounting data access was successfully isolated
🚫 Cross-department application misuse was blocked
📏 System state now meets confidentiality + business separation requirements

🔥 Impact

This change reduced internal data exposure risk by ensuring that:

Only the right users access the right applications

Sensitive finance and HR data is not accessible across departments

Business role boundaries are enforced through policy, not trust

This directly supports HIPAA, SOX, and Principle of Least Privilege internal controls.

🧩 NICE Framework Alignment
Category	Code	Skill Demonstrated
Task	T0123	Implement cybersecurity countermeasures
Knowledge	K0060	Operating system security configuration
Ability	S0031	System access control implementation
Skill	S0147	Assessing effectiveness of applied controls
🏁 Summary

This challenge demonstrates real-world identity-based access enforcement using Windows Server and AppLocker to prevent improper internal data access — a core requirement in enterprise SOC and IAM roles.
