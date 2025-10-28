# 🪟 Windows Security Administration Lab – EFS, BitLocker & Updates

**Course:** CIS1950 – Windows Client Administration  
**Author:** Frankie Lopez  
**Environment:** Windows 10 VM | PowerShell | Active Directory Tools  

---

## ⚙️ Objective
Implement and validate Windows data protection controls using **file and disk encryption**, **certificate recovery**, and **system patch management** to ensure confidentiality, integrity, and recoverability.

---

## 🧰 Tasks Completed
- Configured **Encrypting File System (EFS)** to protect user-sensitive files  
- Tested **cross-user access restrictions** to validate permission enforcement  
- Performed **certificate recovery** using a **Recovery Agent** and certificate import  
- Enabled and verified **BitLocker** full-disk encryption with **Recovery Key backup**  
- Confirmed BitLocker status and administration using PowerShell (`Get-Command *BitLocker*`)  
- Managed **Windows Updates** to maintain system integrity and patch compliance  

---

## 🛡️ Security Purpose
These configurations enforce:
- **Confidentiality** of stored files and disks
- **Recovery capability** in the event of key loss or device theft
- **System trustworthiness** through ongoing security patch management

This reflects **real enterprise workstation hardening practices**.

---

## 🧠 Key Skills Demonstrated
| Skill Category | Description |
|----------------|-------------|
| Windows Security Administration | Implemented system-level security controls |
| Encryption & Key Management | Used EFS and BitLocker with recovery strategies |
| Certificate Services | Managed identity-based encryption certificates |
| PowerShell Operations | Verified encryption and system state through CLI |
| Patch Compliance | Ensured system was fully updated and hardened |

---

## 🧩 Framework Alignment

**NICE Framework (NIST SP 800-181):**
- **T0123:** Implement cybersecurity controls for systems and applications  
- **T0276:** Apply hardening techniques to reduce attack surface  
- **K0060:** OS-level security configuration and auditing  

**MITRE ATT&CK:**
| Technique | Description |
|----------|-------------|
| **T1562.001** | Modify security tools (BitLocker policy & key mgmt) |
| **T1552** | Credentials in files / encryption protection (EFS) |
| **T1078** | Valid accounts and role-based access testing |

---

## 📊 Outcome
- **File-level and disk-level encryption fully configured**
- **Recovery keys validated and stored securely**
- **Unauthorized access attempts were blocked**
- **System confirmed patched and current**

✅ **Result:** Secure workstation configuration aligned with enterprise hardening standards.


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

