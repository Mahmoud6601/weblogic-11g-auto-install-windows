# **Oracle WebLogic 11g – Automated Installation**

This repository contains all the necessary resources and a **PowerShell automation script** for installing **Oracle WebLogic 11g** along with its required components (Java JDK, Weblogic server, Forms & Reports, Web Tier), including essential configuration steps.

---

## Features
- Installs **Java JDK** silently.
- Prepares all **prerequisites** for WebLogic installation.
- Launches the WebLogic installer for manual selection of installation type.
- Configures the **environment** automatically after installation.

---

## 📂 Repository Structure
```
forms&reports/       # Oracle Forms & Reports installer files
jdk/                 # Java Development Kit installer files
webtier/             # Web Tier installer files
wls/                 # WebLogic Server installer files
auto_wls_setup.ps1   # PowerShell script for automated setup
```

---

## Prerequisites
Before running the installation script, ensure:

| Requirement | Description |
|-------------|-------------|
| **Static IP** | Server must use a static IP address (not DHCP). |
| **Installation Directory** | Place all installer folders under `C:\weblogic\`. |
| **Administrator Privileges** | Run the script with elevated privileges. |

---

## Installation
1. **Download or Clone** this repository:
   ```powershell
   git clone https://github.com/Mahmoud6601/weblogic-11g-auto-install-windows.git
   ```

2. **Move Installation Files** to:
   ```
   C:\weblogic\
   ```
   *(Ensure all folders: `forms&reports`, `jdk`, `webtier`, `wls` are inside.)*

3. **Run the Script** as Administrator:
   ```powershell
   Set-ExecutionPolicy Bypass -Scope Process -Force
   .\auto_wls_setup.ps1
   ```

4. **Follow On-Screen Instructions** when the WebLogic installer launches.

---

## 📄 Additional Notes
- Detailed steps are in **`WebLogic_Installation_Guide.pdf`**.
- Tested on **Windows Server** environments.
- Ensure there are no conflicting Java installations.
- Verify sufficient disk space and permissions before installation.
