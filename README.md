
# 🛡️ MYDFIR 30-Day Microsoft Challenge


## 📘 Table of Contents
- [🎯 Purpose](#-purpose)
- [📘 Project Overview](#-project-overview)
- [Current SOC Diagram](#current-soc-diagram)
- [🧰 Current Lab Environment](#-current-lab-environment)
- [🔍 What I Built and Investigated](#-what-i-built-and-investigated)
- [🏁 Summary of Results](#-summary-of-results--week-1)

## 🎯 Purpose

I recently joined the **MyDFIR SOC Communty Program**, which is designed to help participants gain **hands-on experience** and develop **job-ready cybersecurity skills** through practical labs, guided projects, and real-world simulations.  

As part of this journey, I’m sharing my work on the **Microsoft 30-Day Challenge**, one of several projects within the program. 

By documenting my progress, I aim to showcase my technical growth, demonstrate my ability to apply SOC concepts in real-world scenarios, and strengthen my expertise in cybersecurity operations.


---

## 📘 Project Overview
This repository documents my progress in the **Microsoft 30-Day Challenge**, where I’m building and managing a **cloud-based  (SOC)** from scratch using **Microsoft Sentinel** and other Microsoft security tools.

The goal of this challenge is to gain hands-on experience in modern cloud SOC operations from environment setup to incident investigation and response, with a focus on phishing analysis, threat detection, and incident reporting.

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
- Create Log Analytics Workspace


---
## Current Soc Diagram
![SOC Lab Architecture](Soc-Arch-Diagram.png)

## 🧰 Current Lab Environment
- **Cloud:** Microsoft Azure (Subscription: *abdou*****@.onmicrosoft.com*)  
- **SOC:** Microsoft Sentinel (Workspace: *Mydfir-abdou*)  
- **Resource Group:** (mydfir-challenge)
- **Endpoint:** 1 Windows VM (windows11)
- **Network:** VNet (windows11-vnet/default)
- **Roles:** SOC Analyst role  
- **Log Analytics:** (Mydfir-abdou-law)

**Connected Data Sources:**  
- Microsoft 365  
- Defender for Endpoint  
- XDR (Extended Detection and Response) from Microsoft Content Hub

---

### 🔍 What I Built and Investigated
- Deployed and configured a **Microsoft Sentinel workspace** connected to Azure resources  
- Integrated **Defender for Endpoint** and **XDR** data connectors  
- Created a **custom SOC dashboard** for log visibility (Screenshots in `Dahsboards/screenshots`)  
- Investigated a **brute-force attack simulation** and documented findings  

---

## 🏁 Summary of Results — Week 1

### 💡 What I Can Do Now
- Deploy and configure a **Microsoft Sentinel SOC** with connected data sources  
- Build **custom dashboards** and write **KQL queries**  
- Connect and manage **data connectors** (Defender for Endpoint, XDR)
- Build and customize **SOC dashboards** for visibility and monitoring.
- Document and report **incidents** 

### 🌟 Most Impactful Experience
Investigating my first simulated **brute-force attack** using Sentinel data, seeing how logs, alerts, and detections connect in a real SOC environment.

### 🚀 Areas for Improvement
- Expand my **KQL query skills** for deeper investigations.  
- Investigate **Phishing Email**  
- Develop **automated playbooks (Logic Apps)** for faster incident response.  
- Continue improving my **incident documentation and report writing**.

---



