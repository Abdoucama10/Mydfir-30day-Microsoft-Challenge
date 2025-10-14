
# 🛡️ MyDFIR 30-Day Microsoft Challenge

## 🎯 Purpose
I’m sharing this project to demonstrate my passion for cybersecurity by publishing my learning journey and hands-on projects.  
I aim to show continuous learning through practical, real-world labs that teach a Cloud SOC workflow.

---

## 📘 Project Overview
This repository documents my progress in the **Microsoft 30-Day Security Challenge**, where I’m building and managing a **cloud-based Security Operations Center (SOC)** from scratch using **Microsoft Sentinel** and other Microsoft security tools.

The goal of this challenge is to gain **hands-on experience** in modern cloud SOC operations — from environment setup to incident investigation and response.

**Tools used**
- Microsoft Sentinel  
- Microsoft Azure  
- Microsoft Defender for Endpoint  
- Microsoft 365 Security  

**Skills practiced**
- SOC environment setup and configuration  
- KQL (Kusto Query Language) for detection & hunting  
- Incident investigation and reporting  
- Install Microsoft Defender XDR connector
- Create Analytics rule in Defender XDR


---
## Current Soc Diagram
![SOC Lab Architecture](Soc-Arch-Diagram.png)

## 🧰 Current Lab Environment
- **Cloud:** Microsoft Azure (Subscription: *abdou*****@.onmicrosoft.com*)  
- **SOC:** Microsoft Sentinel (Workspace: *Mydfir-abdou*)  
- **Resource Group:** (mydfir-challenge)
- **Endpoints:** 1 Windows VM (windows11)
- **Network:** VNet (windows11-vnet/default)
- **Roles:** SOC Analyst role  
- **Log Analytics:** (Mydfir-abdou-law)
- - **Connected Data Sources:**
  - Microsoft 365
  - Defender for Endpoint
  - **XDR (Extended Detection and Response) from Microsoft Content Hub**

---

## 📦 Resources Created So Far
- [x] Azure Subscription  
- [x] Log Analytics Workspace  
- [x] Microsoft Sentinel workspace  
- [x] Connected Data Connectors: Microsoft 365, Defender for Endpoint, Entra ID  
- [x] Custom Workbook / Dashboard (Screenshots in `/Screenshots`)  
- [x] Bookmarks for investigations  
- [x] Initial KQL queries and saved queries  
- [ ] Playbooks / Automation (planned)  
- [ ] Threat intelligence connector (planned)
- [ ] Email Investigations 

---



