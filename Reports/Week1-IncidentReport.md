## 🕵️‍♂️ Microsoft 30-Day Challenge — Day 7 Incident Report

### 1. 🧩 Findings
**Date & Time:** 2025-10-08, 16:14:42 UTC  
**Target:** Administrator variant accounts  
**Failed Logons:** 16,110  
**Successful Logons:** None detected  
**Affected Hosts:**  
- SOC-FW-RDP → 10,122 attempts  
- SHIR-Hive → 2,778 attempts  
- SHIR-SAP → 55 attempts  
**Source IPs:** Not captured in available logs  
**MITRE ATT&CK Alignment:**  
- **T1110 — Brute Force**  
- **T1021 — Remote Services (RDP)**

---

### 2. 🔍 Investigation Summary
Multiple failed logon attempts (**Event ID 4625**) were detected targeting Administrator variant accounts, suggesting a brute-force attack focused on privileged credentials.

- A **KQL query** measured failed logons between the first and last attempt, revealing **12,955 failed attempts** within a short time frame — consistent with automated activity.  
- No successful logins (**Event ID 4624**) were recorded for these accounts.  

| Element | Detail |
|----------|---------|
| **WHO** | Suspected external actor based on attack behavior (source not confirmed) |
| **WHAT** | Automated brute-force attack via RDP |
| **WHEN** | 2025-10-08, 16:14:42.267 – 16:14:42.595 UTC |
| **WHERE** | SOC-FW-RDP, SHIR-Hive, SHIR-SAP |
| **WHY** | Attempt to gain unauthorized administrative access |
| **HOW** | Rapid, automated password-guessing script/tool |

---

### 3. 🧠 MITRE ATT&CK–Based Recommendations

| ID | Mitigation | Summary |
|----|-------------|---------|
| **M1036** | Account Use Policies | Apply account lockout policies after multiple failed attempts; implement conditional access for risky logins. |
| **M1032** | Multi-Factor Authentication | Enforce MFA for all privileged and external accounts. |
| **M1027** | Password Policies | Use strong, unique passwords following NIST standards; block known breached credentials. |
| **M1018** | User Account Management | Reset targeted accounts, review admin privileges, disable unused or shared accounts. |

---

### 4. 🧾 Analyst Notes
- The incident demonstrates how brute-force activity can be quickly detected using Microsoft Sentinel’s event correlation.  
- KQL queries were instrumental in identifying event patterns and timing.  
- No lateral movement or privilege escalation observed in this stage.

---

### 5. 📊 4. Screenshots & Evidence
Attach relevant screenshots below: 

Failed Logon per accounts

<img width="900" height="403" alt="image" src="https://github.com/user-attachments/assets/f8084244-af0a-42d5-836e-f16be813a6f3" />


Timeframe between the first and last attempt and attempts counts
<img width="934" height="343" alt="image" src="https://github.com/user-attachments/assets/47dc16f5-9708-4cb6-9c9e-1ceb7153cd0a" />


Failed attempts per Hosts 

<img width="900" height="325" alt="image" src="https://github.com/user-attachments/assets/28ee17c1-30cd-468f-9550-ccc526dce54c" />



