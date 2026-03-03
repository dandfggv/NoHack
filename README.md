<p align="center">
  <img src="Ico/No hack.ico" width="128" height="128" alt="NoHack Icon">
</p>

<h1 align="center" style="color:#ffffff;">NoHack Anti‑Cheat Suite</h1>

<p align="center" style="color:#cccccc;">
A lightweight, modular Windows anti‑cheat system designed for modern games.<br>
This README is optimized for GitHub dark mode.
</p>

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

## 🌙 Overview

NoHack Anti‑Cheat protects Windows games by monitoring integrity, validating DLLs, detecting suspicious processes, and maintaining secure logs. The suite installs into Program Files and stores logs in ProgramData, following professional Windows software standards.

## 📦 Installed Components

**Install Location:**  
C:\Program Files\NoHack Anti-Cheat\

### Main Application
**NoHack.exe**  
• Monitors game integrity  
• Scans for blacklisted processes  
• Validates DLL hashes  
• Logs activity  
• Runs silently in the tray  

## 🧰 Tools (Installed in Tools\)

**IntegrityGen.exe**  
Generates CRC32 integrity lists for game files.

**LogViewer.exe**  
Views logs stored in:  
C:\ProgramData\NoHack\logs\

**NoHackConfigGen.exe**  
Creates JSON configs and integrity templates.

**NoHackControl.exe**  
GUI control panel for profiles, logs, and settings.

**ProfileSelector.exe**  
Launches NoHack with a chosen profile.

**NoHackPlugin.dll**  
Optional safe plugin DLL for game‑side communication.

## 📁 Folder Structure

C:\Program Files\NoHack Anti-Cheat\
│  
├── NoHack.exe  
├── Readme.txt  
├── Ico\  
│   └── No hack.ico  
│  
└── Tools\  
    ├── IntegrityGen.exe  
    ├── LogViewer.exe  
    ├── NoHackConfigGen.exe  
    ├── NoHackControl.exe  
    ├── ProfileSelector.exe  
    └── NoHackPlugin.dll  

Logs are stored in:  
C:\ProgramData\NoHack\logs\

## 🖥️ Start Menu Shortcuts

Start Menu  
 └── NoHack Anti-Cheat  
      ├── NoHack Anti-Cheat  
      ├── Tools Folder  
      ├── IntegrityGen  
      ├── LogViewer  
      ├── NoHackConfigGen  
      ├── NoHackControl  
      ├── ProfileSelector  
      └── Logs Folder  

A desktop icon can be created during installation.

## 🚀 Running NoHack

Launch via Start Menu or run:  
C:\Program Files\NoHack Anti-Cheat\NoHack.exe

On first launch, NoHack asks for the game executable. After setup, it will:  
• Verify game integrity  
• Monitor suspicious processes  
• Validate DLLs  
• Log all activity  

## 📝 Creating Integrity Files

Generate integrity lists:

IntegrityGen.exe default game.dll engine.dll plugins\core.dll

This produces:

integrity_default.txt

Place this file next to NoHack.exe or inside the game folder.

## 🧩 Creating JSON Config Files

Use NoHackConfigGen.exe to generate:  
• nohack_config.json  
• nohack_integrity_<profile>.txt  

Place these inside the game directory.

## 🛠️ PATH Integration

The installer automatically adds:

C:\Program Files\NoHack Anti-Cheat\Tools

to your PATH so tools can run from any terminal.

## 📚 License

This project is provided as‑is for educational and personal use.

## 🙋 Support

For updates or improvements, contact the developer or check the repository.
