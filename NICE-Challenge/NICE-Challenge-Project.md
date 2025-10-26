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

