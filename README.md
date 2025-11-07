# 🛡️ SentinelDevOps

**SentinelDevOps** brings DevOps automation to **Microsoft Sentinel**.  
It’s a framework to **deploy, track, and maintain Sentinel playbooks** using CI/CD pipelines and GitOps principles — making security automation repeatable, auditable, and version-controlled.

---

## 🚀 Overview

In most SOC environments, playbooks are manually deployed and easily fall out of sync across environments.  
**SentinelDevOps** solves that by integrating Sentinel with **DevOps workflows** — enabling automated deployments and configuration tracking.

**Core idea:**  
> Treat security automation like software — version-controlled, tested, and continuously delivered.

---

## ⚙️ Features

- 🧩 **CI/CD Integration** — Deploy Sentinel playbooks automatically through GitHub Actions or Azure DevOps.  
- 🔄 **GitOps Model** — Every change is tracked through commits and pull requests.  
- 🧠 **Automated Tracking Table** — Maintains real-time visibility of playbook deployments.  
- 📦 **Infrastructure-as-Code (IaC)** — Define and manage Logic Apps and Sentinel configurations through ARM templates or JSON.  
- 🔐 **Security-as-Code** — Enforce consistent, auditable automation across environments.

---

## 🧰 Tech Stack

| Component | Description |
|------------|-------------|
| **Microsoft Sentinel** | SIEM/SOAR platform |
| **Azure Logic Apps** | Underlying automation engine for playbooks |
| **GitHub Actions / Azure DevOps** | CI/CD automation pipelines |
| **ARM Templates / JSON** | Infrastructure-as-Code definition |
| **Tracking Table** | Automatically updated table of playbooks and deployments |

---

## 🧭 Architecture

1. **Source Control:** All playbooks are stored as JSON in GitHub.  
2. **CI/CD Trigger:** On each commit, the pipeline validates and deploys changes.  
3. **Deployment:** Logic Apps are deployed to Sentinel via ARM templates.  
4. **Tracking Table:** Updated automatically to reflect the current state of deployments.

---

## 🧑‍💻 How to Use

1. **Clone the repository**
   ```bash
   git clone https://github.com/jayWaikato/SentinelDevops.git


## 📚 Sources / References


- [Azure Sentinel GitHub Repository](https://github.com/Azure/Azure-Sentinel/tree/master)  
  *Used as a reference for existing playbook structures, ARM templates, and best practices for Sentinel automation.*  

- [Analytics Rules Exchange](https://analyticsrules.exchange/)  
  *Guided the creation of sample analytics rules and detection logic for SOC scenarios.*  

- [KQL Threat Hunting Queries](https://github.com/cyb3rmik3/KQL-threat-hunting-queries)  
  *Adapted and customized queries for automated incident triage and monitoring within the CI/CD pipeline.*  
