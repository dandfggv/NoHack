# NoHack Anti‑Cheat Suite

NoHack Anti‑Cheat is a modular Windows security system designed to protect games from tampering, unauthorized tools, and integrity violations. It includes a complete toolchain for configuration, integrity generation, log viewing, and profile management. The suite installs cleanly into Program Files and stores logs in ProgramData, following professional Windows software standards.

## Installed Components

After installation, the suite is located in:

C:\Program Files\NoHack Anti-Cheat\

### Main Application
NoHack.exe  
The core anti‑cheat engine.  
• Monitors game integrity  
• Scans for blacklisted processes  
• Validates DLL hashes  
• Logs activity  
• Runs silently in the system tray  

## Tools (Installed in Tools\)

IntegrityGen.exe  
Generates integrity files (integrity_<profile>.txt) containing CRC32 hashes of game DLLs and executables.

LogViewer.exe  
GUI tool for browsing logs stored in:  
C:\ProgramData\NoHack\logs\

NoHackConfigGen.exe  
Creates JSON configuration files and integrity templates for new game profiles.

NoHackControl.exe  
Control panel for:  
• Managing profiles  
• Setting game paths  
• Opening logs  
• Launching NoHack with a selected profile  

ProfileSelector.exe  
Simple launcher that allows selecting a profile and starting NoHack with it.

NoHackPlugin.dll  
A safe plugin DLL that can be loaded by your own game (not injected). Used for optional heartbeat or communication features.

## Folder Structure

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

## Start Menu Shortcuts

The installer creates a Start Menu folder:

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

## Running NoHack

To launch the anti‑cheat:  
• Use the Start Menu shortcut, or  
• Run NoHack.exe directly from Program Files.

On first launch, NoHack will ask you to select the game executable. After configuration, NoHack will:  
• Verify game integrity  
• Monitor for suspicious processes  
• Validate DLL hashes  
• Log all activity  

## Creating Integrity Files

Use IntegrityGen.exe:

IntegrityGen.exe default game.dll engine.dll plugins\core.dll

This produces:

integrity_default.txt

Place this file next to NoHack.exe or inside the game folder depending on your setup.

## Creating JSON Config Files

Use NoHackConfigGen.exe to generate:  
• nohack_config.json  
• nohack_integrity_<profile>.txt  

These files can be placed inside the game directory.

## PATH Integration

The installer automatically adds:

C:\Program Files\NoHack Anti-Cheat\Tools

to the user PATH, allowing you to run tools from any command prompt.

## License

This project is provided as-is for educational and personal use.

## Support

For questions, updates, or improvements, contact the developer or check the project repository.
