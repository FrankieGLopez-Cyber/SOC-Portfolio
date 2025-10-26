# 🪟 Windows Security Administration Lab – EFS, BitLocker & Updates

**Course:** CIS1950 – Windows Client Administration  
**Author:** Frankie Lopez  
**Environment:** Windows 10 VM | PowerShell | Active Directory Tools  

---

## ⚙️ Objectives
Implement and test Windows security features to protect data and systems using encryption, key recovery, and patch management.

---

## 🧰 Tasks Completed
- Configured **EFS (Encrypting File System)** to protect sensitive files.  
- Tested **encryption access controls** between users.  
- Recovered **lost encryption keys** using certificate import and recovery agent.  
- Enabled and tested **BitLocker drive encryption** with recovery key backup.  
- Verified **BitLocker management via PowerShell** (`Get-Command *BitLocker*`).  
- Managed **Windows Updates** to ensure system integrity and patch compliance.  

---

## 🧠 Key Skills Demonstrated
- Windows security administration  
- File and drive encryption (EFS, BitLocker)  
- Certificate management (PKI fundamentals)  
- PowerShell automation  
- Patch management and update control  

---

## 🧩 Framework Alignment
**NICE Framework (NIST SP 800-181):**  
- **T0123:** Implement system-level cybersecurity controls for applications and systems.  
- **T0276:** Apply system hardening techniques to reduce attack surface.  
- **K0060:** Knowledge of operating system security configuration and auditing.  

**MITRE ATT&CK Techniques:**  
- **T1562.001 – Disable or Modify Tools (BitLocker Configuration)**  
- **T1552 – Unsecured Credentials (EFS and Key Recovery)**  
- **T1078 – Valid Accounts (User Access & Certificate Management)**

---

## 📊 Outcome
Successfully configured and validated multiple layers of Windows data protection and recovery mechanisms.  
Demonstrated ability to secure client systems using native Microsoft tools and policies.

## Screenshots
### Certificate Recovery
<img width="613" height="457" alt="image" src="https://github.com/user-attachments/assets/f8d1aff9-2e73-4bd4-a7b6-fa11aa85246a" />

<img width="459" height="425" alt="image" src="https://github.com/user-attachments/assets/7777b587-ece1-4fa0-96e9-9f3527bc0f09" />

<img width="455" height="434" alt="image" src="https://github.com/user-attachments/assets/53035b7e-9f23-4fb1-9e40-952817c5d128" />

### BitLocker Encryption via PowerShell
<img width="719" height="527" alt="image" src="https://github.com/user-attachments/assets/91e640be-5467-440c-b350-01417fd6ebc5" />

<img width="687" height="509" alt="image" src="https://github.com/user-attachments/assets/f7326251-e4c3-42b8-8c45-39e7e9a01828" />

### Windows Update Verification
<img width="694" height="650" alt="image" src="https://github.com/user-attachments/assets/6ec79abb-5f9c-4774-affc-12ad1f6a9df8" />

> **Result:** Fully encrypted Windows environment with BitLocker and EFS, validated encryption recovery keys, and verified system updates.

