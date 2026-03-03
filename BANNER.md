##############################################
#                                            #
#        ████  ████   ██   ██   ████         #
#        ██    ██     ██   ██   ██           #
#        ████  ████   ██   ██   ████         #
#        ██    ██      ██ ██    ██           #
#        ████  ████     ████    ████         #
#                                            #
#                N O H A C K                 #
#                                            #
##############################################

<p align="center">
  <img src="Ico/No hack.ico" width="128" height="128" alt="NoHack Icon">
</p>

<h1 align="center" style="color:#ffffff;">NoHack Anti‑Cheat Suite</h1>

<p align="center" style="color:#cccccc;">
A lightweight, modular Windows anti‑cheat system designed for modern games.<br>
Dark‑mode optimized README for GitHub.
</p>

---

## 🌙 Dark‑Mode Friendly Overview

NoHack Anti‑Cheat protects Windows games by monitoring integrity, validating DLLs, detecting suspicious processes, and maintaining secure logs.  
The suite installs into **Program Files** and stores logs in **ProgramData**, following professional Windows standards.

---

## 📦 Installed Components

**Install Location:**  
`C:\Program Files\NoHack Anti-Cheat\`

### Main Application
**NoHack.exe**  
- Monitors game integrity  
- Scans for blacklisted processes  
- Validates DLL hashes  
- Logs activity  
- Runs silently in the tray  

---

## 🧰 Tools (Installed in `Tools\`)

**IntegrityGen.exe**  
Generates CRC32 integrity lists for game files.

**LogViewer.exe**  
Views logs stored in:  
`C:\ProgramData\NoHack\logs\`

**NoHackConfigGen.exe**  
Creates JSON configs + integrity templates.

**NoHackControl.exe**  
GUI control panel for profiles, logs, and settings.

**ProfileSelector.exe**  
Launches NoHack with a chosen profile.

**NoHackPlugin.dll**  
Optional safe plugin DLL for game‑side communication.

---

## 📁 Folder Structure

