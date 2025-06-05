# Manual Windows Update Script (Non-GUI)
### Created by **DadOfTheClan**

---

## 📋 Description

This PowerShell script allows you to manually search, select, and install Windows Updates — including software, drivers, and optional updates — on systems without a GUI. It's perfect for servers, remote systems, automation, or sysadmins who prefer terminal-driven workflows.

---

## 🔧 Features

- List all available updates (software, drivers, firmware, optional).
- Clean tabular output in the console.
- Export update list to CSV and JSON.
- Select updates interactively or use command-line switches for automation.
- Supports reboot control (optional or automatic).
- Silent/Unattended mode available.
- Logs saved to disk for review or auditing.

---

## 💻 Requirements

- Windows 10/11 or Windows Server (with access to Windows Update)
- PowerShell (v5 or higher)
- Internet connection

---

## 🚀 Usage

```powershell
.\Updates.ps1 [-All] [-Software] [-Driver] [-Optional] [-Silent] [-NoRestart]
