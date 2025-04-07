# Practical_jenkins_journey
---
# 🚀 Jenkins: Practical Automation Guide

> *Real-world CI/CD knowledge put to the test – not just theory.*

---

## 🧠 What I Know

- **CI/CD Flow**: Code → Source Control → Build → Test → Package → Deploy  
- **CI** = Package the code  
- **CD** = Auto-deploy the package  

---

## ⚙️ Jenkins Essentials

- **Port**: `8080` (Change via `/etc/default/jenkins`)
- **Initial Password**: `/var/lib/jenkins/secrets/initialAdminPassword`
- **Install Options**:  
  - Dedicated server (AWS/GCP)  
  - Local service (`systemctl status jenkins`)  
  - Docker container

- **Plugins**: Seamlessly integrate tools (e.g., Docker plugin)

---

## 📂 Key Jenkins Files

- `/var/lib/jenkins/` → 🔐 Back it up!
  - `config.xml` → Core settings
  - `credentials/` → Secrets
  - `jobs/` → Build configs, history, workspace
  - `plugins/` → Downloaded integrations
  - `nodes/` → Optional agent configs

> In Docker: Home becomes `/var/jenkins_home`

---

## 🔐 Credentials

- Created via: *Manage Jenkins → Credentials → Global*
- Tip: IDs must not contain spaces
- AWS plugin adds support for cloud credentials

---

## 👷 Job Types

1. **Freestyle Jobs**:  
   - Good for parameterized inputs  
   - Use GitHub Webhooks for auto triggers

2. **Pipeline Jobs**:  
   - Written in **DSL (Groovy)**  
   - Support **Declarative** & **Imperative** syntax  

---

## 🛠️ Power Features in Pipelines

- **Build Discarder**: Clean up old builds  
- **Checkout**: Pull from GitHub  
- **Tools**: Use Maven or others easily  
- **Env Variables**: Dynamic & secure configs  
- **Parameterized Builds**: Runtime flexibility  
- **Upstream/Downstream**: Job chaining  
- **Post Actions**: Notifications (success/failure)  
- **Built-in Vars**: `$BUILD_ID`, `$JOB_NAME`, etc.  
- **Scripts & Loops**: Advanced logic in Groovy  
- **Functions**: Reuse logic cleanly  
- **Script from File**: Run external Python/Bash

---

## 🐳 Jenkins + Docker = ❤️

> Built & deployed Jenkins in a Docker container — full control, fast setup, clean testing environments.

---

## 👋 Why This Matters

This isn’t just a Jenkins crash course — it’s my **hands-on foundation** for modern DevOps.

I’m building this repo to stand out by sharing *real, applied knowledge* — no fluff.

