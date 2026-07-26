<img width="3836" height="2160" alt="LollozzOsWallpaper" src="https://github.com/user-attachments/assets/95617af1-f553-4a52-8db2-647c3977d10a" />







# LollozzOS Configurator

Welcome, I created this utility that integrates every possible optimization for Windows 10/11. The utility was created by me (Lollozz), a computer and software enthusiast in general, and I've tested everything on my PC.
The interface is clean and you can navigate using the on-screen numbers. Each section is explained by pressing the corresponding number, so you can see what the script does before applying it. Happy debloating!!

## 🖥️ Interface

- CLI menu entirely in Italian, with dedicated ASCII art banners for each module and a differentiated ANSI color scheme (blue, green, red, yellow, purple) to quickly identify the section you're in.
- Numbered menu navigation with input validation and error handling.

- Each module includes a "What does it do?" entry with detailed technical documentation for each optimization.
- Integrated licensing system with verification starting from the home screen.

---

## 🔐 License

LollozzOS is protected by a proprietary licensing system tied to the hardware of the PC on which it is activated.

**To request a license**: join the Discord channel and message me directly.

- Discord: https://discord.gg/gd5cT3Jw9M

---

## ⚙️ Main Menu — Windows Optimizer Ultimate Edition

1. **Windows** – Opens Windows Manager (debloat, privacy, repair, activation)
2. Office installation and activation **Create Restore Point** – Restore Manager
3. **Download Browsers and Apps
4. **Choose Your Game** – Game Config Manager (Warzone, Fortnite)
5. **Update and Optimize GPU** – NVIDIA/AMD dedicated tweaks
6. **Other Optimizations** – (other tweaks)
7. **Optimize Storage/RAM** – Disk & RAM Manager
8. **System Information**
9. **Set Power Profile** – Power Manager
10. **USB Overclock** – Polling Rate and Peripheral Calibration
11. **Timer Resolution** – Kernel-level Input Lag Reduction
12. **Optimize Network
13. **Office Tool** –
14. **Manage BIOS** – BIOS Manager
15. **My Social Networks**
16. **Exit**
---

## 🌐 Network Optimizer

Module dedicated to in-depth optimization of the network stack, complete with technical documentation integrated into the program:

- **Deep Reset** of interfaces, Winsock, IP, TCP, Teredo, 6to4, firewall, and DNS cache
- **Gaming Priority**: Tuning `NetworkThrottlingIndex`, `SystemResponsiveness`, and priority of multimedia/game processes in the system scheduler
- **Bandwidth Limit Removal**: Elimination of QoS, SMB, and Task Offload throttling, optimization of AFD (Ancillary Function Driver) parameters
- **TCP NoDelay** (Nagle algorithm disabled) applied to all interfaces to reduce ping and jitter
- **Advanced Global TCP Tuning** via `netsh`: autotuning, ECN, RSS, CTCP congestion provider, Fast Open, heuristics deactivation, and RSC
- **Network Driver Optimization**: Automatic detection of the active adapter and deactivation of power-saving/latency parameters (Gigabit auto-disable, DMA Coalescing, etc.), with automatic driver backup before each change
- **DNS Manager**: Active network adapter detection, quick Cloudflare/Google DNS setup, or DHCP reset, with integrated latency test
- **Diagnostic Tools**: Quick links to Speed ​​Test, Bufferbloat Test, and Packet Loss Test
- Automatically launches dedicated external tools (TestMb, TCP Optimizer) after optimization is complete

---

## 🎮 USB Overclock

- **Polling Rate Overclock** of USB peripherals (up to 1000Hz+) to reduce sampling delay and click-to-photon latency
- **Analog Pad Calibration** via integration with dedicated online tools
- Automatic creation of shortcuts in the desktop context menu for quick access to overclocking and calibration
- Management via a dedicated external tool with automatic permission elevation

---

## ⏱️ Timer Resolution

- Set the **System Timer** to 0.5ms** (versus the Windows standard of 15.6ms) to dramatically reduce input lag
- Check the currently active timer resolution
- Automatically back up used tools and create an auto-start shortcut
- Automatically generated restore script to return to default values

---

## 🔋 Power Manager

- Import a **Custom Power Profile** optimized for performance
- Completely restore Windows power plans and default power settings
- Check CPU **Core Parking** (to ensure all cores are active and available)

---

## 🎨 GPU Tweaks (NVIDIA / AMD)

- Dedicated and separate paths for **NVIDIA cards (GeForce)**, **AMD (Radeon Adrenalin)**, and **INTEL**
- "Deep" registry tweaks to optimize GPU drivers and performance
- Desktop extraction of dedicated utilities for the detected manufacturer

- ## 💾 Disk & RAM Manager

- Launch *Windows Memory Cleaner* to free up occupied RAM
- Launch *ISLC* (Intelligent Standby List Cleaner), copied and stored in a dedicated folder on C:\LollozzOs
- *NVMe latency optimization* by enabling Native NVMe parameters in the registry
- Integrated documentation on I/O optimization, TRIM, and texture loading micro-stutter reduction

---

## 🧬 BIOS Manager

- *BIOS Update Wizard*: Automatically detects motherboard manufacturer and model, installed BIOS version and date, with direct search for the latest available update
- *Direct reboot to BIOS/UEFI* from a single menu item
- *Unlock hidden BIOS settings* via NVRAM Export/Import
- Dedicated "Reboot to BIOS" shortcut installable in the desktop context menu

---

## 🔄 Restore Manager

- Create a *restore point* before each optimization session
- Complete list of available restore points, with dedicated log
- Directly launch a restore point from the menu
- Information section on restore point usage and best practices

---

## 📎 Office Manager

- *Microsoft Office* installation wizard
- Office activation integrated into the same module

---

## 🕹️ Game Optimization 

"Choose Your Game" module to apply ready-to-use configurations directly to your game files:

- *Import of ready-made optimized configs*, automatically saved to the correct path in the game's user files
- *Backup and restore* of the current configuration before any changes, to ensure full reversibility
- Dedicated support for *Warzone, including download and automatic configuration of the **Audio Mod*, designed to improve the perception of footsteps and directional sounds in-game
- Integrated technical documentation for each supported game
- Ability to enable custom resolutions via CRU
---

## 🎥 OBS Studio Module 

Standalone module integrated into the main menu that manages the entire OBS Studio lifecycle:

- Automatic installation via Winget/Chocolatey with error handling
- *Setup Wizard*: GPU detection, resolution selection (including default values) Custom/Fractional), FPS, connection type, automatic profile generation, JSON scene (Monitor/Mic/Webcam), and dynamically calculated CBR bitrate
- *Debloat OBS*: Removal of non-Italian/English localization files, CEF language pack cleaning, unnecessary theme removal, cache/log/crash cleaning
- Configuration reset and complete uninstallation

---

## ⚙️ Windows Manager (debloat and privacy submenu)

1. *Activate Windows*
2. *LollozzOS Extra Settings*
3. *Critus Tech* – dedicated debloat/optimization tools
4. *Debloat Extra*
5. *Other Optimizations*
6. *Ultimate Windows Tweaker*
7. *Remove Windows AI* (Copilot and built-in AI components)
8. *Repair Windows*
9. *Disable Windows Privacy* (based on O&O ShutUp10)
10. *Search/Taskbar Manager*
11. *Integrated Win11Debloat*
12. *Browser Download*
13. *Playbook Installation* (extra tools and configurations package)
14. *CPU Chipset Update* (AMD/Intel auto-detection)
15. *Debloat Chrome*
16. *Debloat Discord*
17. *OBS Studio Management*
18. *Autoruns* (Sysinternals)
19. Integrated Info/Changelog ("What does it do?")

### Areas of focus in detail

- *Telemetry and Privacy*: Completely disable DiagTrack, CEIP, WER, PerfTrack, Microsoft Account settings sync, Timeline/Activity Feed, voice data collection, KMS telemetry
- *Services and Drivers*: Disable non-essential services (OneSyncSvc, TrkWks, PcaSvc, UCPD, etc.) and background drivers (GpuEnergyDrv, NetBT)
- *Registry*: Hundreds of HKLM/HKCU tweaks applied to both the current user and the Default profile (for future new accounts), with custom LollozzOS branding in winver and boot entry
- *Bloatware Removal*: Uninstall pre-installed AppX apps, block automatic reinstallation, remove OneDrive, Xbox, Cortana/Extended Search, LockApp, SmartScreen, sync programs
- *Gaming & Performance*: Game Mode, 90% CPU priority for the active app, disabling Page Combining, removing SMB limits for LAN, resolution/refresh rate management
- *Security/Defender*: Dedicated menu for controlled disabling of Windows Defender with automatic pre-change backup of services
- *Maintenance*: Automatically generated restore scripts before each critical change, to ensure reversibility

---

## 🛠️ Tweaks

Windows Manager submenu that brings together 17 targeted and individually selectable tweaks in a single panel, for granular control without having to go through a full debloat:

1. *Disable Windows Driver* – disable non-essential background drivers
2. *Disable Microsoft Apps* – remove pre-installed system apps
3. *Optimize Games/Apps* – prioritize and allocate resources to foreground processes
4. *Disable Microsoft Edge* – block auto-start and background processes
5. *Remove OneDrive* – complete uninstallation
6. *Remove Lock App* – disable the lock screen
7. *Remove SmartScreen*
8. *Disable Core Isolation/VBS* – disable security virtualization to recover CPU performance
9. *Disable Startup* – clean up auto-start programs
10. *Manage Windows Defender*
11. *Uninstall Microsoft Store*
12. *Disable Hibernation*
13. *Optimize Visual Settings* – disable unnecessary graphical effects
14. *Disable Telemetry*
15. *Set Priority Separation* – tune the CPU scheduler to favor foreground apps
16. *Set Shortcuts* – create shortcuts to utilities
17. *Disable Mitigations* – controlled deactivation of kernel security mitigations (Spectre/Meltdown, SEHOP, Control Flow Guard, DEP) to reduce performance overhead, with dedicated overrides to ensure compatibility with anti-cheat software for major games

Each option applies the change independently and reversibly, so the user can choose exactly which optimizations to enable without affecting the rest of the system.

---

## 🧩 Technical Architecture

- Windows executable (.exe) with console interface and modular menu navigation
- Integrated PowerShell logic for advanced registry, WMI, and GPU management operations
- Dynamically generated restore scripts (rollback) before each invasive change
- Multi-user management: Apply changes to both the current user and the Windows Default profile

---

## ⚠️ Note

LollozzOS Configurator makes profound changes Registry, services, and system components. It is recommended to create a restore point before use and run the application with administrator privileges.

---

## 🙏 Credits

LollozzOS Configurator was also created thanks to the integration of several open source projects available on GitHub, including:

- Chris Titus Tech's Windows Utility
- RemoveWindowsAI Zoocware
- Microsoft Activation Script (MAS)
- Win11Debloat Raphire
- DiscordDebloater insovs

---

##

---

## 🌍 Website

[Insert link to the official website here]

## 🔗 Community

- Discord: https://discord.gg/gd5cT3Jw9M
- TikTok: https://www.tiktok.com/@lollozz_os?_r=1&_t=ZN-98MDYenbJBu
- Instagram: https://www.instagram.com/lollozz_labs?igsh=dnRuYzB0dXQwNDZh&utm_source=qr

- 

