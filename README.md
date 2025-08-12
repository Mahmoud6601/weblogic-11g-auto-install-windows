# **Oracle WebLogic 11g – Automated Installation**

This repository contains all the necessary resources and a **PowerShell automation script** for installing **Oracle WebLogic 11g** along with its required components (Java JDK, Web Tier, Forms & Reports), including essential configuration steps.

---

## 📥 Download WebLogic Installer
The WebLogic installation package is available via MediaFire.  
Download all required parts and extract them into `C:\weblogic\` before running the script.

- **Download Link:** [WebLogic_11g_Installer.zip](https://www.mediafire.com/file/c2ja8xtawc5jtvg/weblogic-11g-installation-automation-windows.rar/file)  
  

---

## 🚀 Features
- Installs **Java JDK** silently.
- Prepares all **prerequisites** for WebLogic installation.
- Launches the WebLogic installer for manual selection of installation type.
- Configures the **environment** automatically after installation.

---

## 📂 Repository Structure
```
forms&reports/       # Oracle Forms & Reports 11g installer files
jdk/                 # JDK installer files (Java Development Kit)
webtier/             # Oracle Web Tier 11g installer files
wls/                 # Oracle WebLogic Server 11g installer files
Install-WebLogic-Win.pdf    # Installation and configuration guide in PDF format
auto_wls_setup.ps1   # PowerShell script to automate WebLogic, Forms, Reports, and Web Tier installation
```

---

## 🛠 Prerequisites
Before running the installation script, ensure:

| Requirement | Description |
|-------------|-------------|
| **Static IP** | Server must use a static IP address (not DHCP). |
| **Installation Directory** | Place all installer folders under `C:\weblogic\`. |
| **Administrator Privileges** | Run the script with elevated privileges. |

---

## ⚙️ Installation

1. **Download the WebLogic Installer** from the link above and place the extracted folders into:
   ```
   C:\weblogic\
   ```
   *(Ensure all folders: `forms&reports`, `jdk`, `webtier`, `wls` are inside.)*

2. **Run the Script** as Administrator:
   ```powershell
   Set-ExecutionPolicy Bypass -Scope Process -Force
   .\auto_wls_setup.ps1
   ```

3. Follow the steps outlined in the PDF guide **Install-WebLogic-Win.pdf** included in this repository.

---

## 📄 Additional Notes
- Detailed steps are in **`Install-WebLogic-Win.pdf`**.
- Tested on **Windows Server** environments.
- Ensure there are no conflicting Java installations.
- Verify sufficient disk space and permissions before installation.
