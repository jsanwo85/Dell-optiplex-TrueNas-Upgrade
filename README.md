# Dell OptiPlex 3020 NAS Upgrade Project

## Overview
This project documents the upgrade and transformation of a Dell OptiPlex 3020 desktop PC into a TrueNAS SCALE-powered Network Attached Storage (NAS) device. The goal was to repurpose an old PC into a cost-effective, fully functioning personal cloud solution with centralized storage and sharing capabilities.

## Objectives
- Upgrade an outdated Dell PC with new hardware components.
- Install and configure TrueNAS SCALE for LAN-based storage access.
- Set up secure SMB shares for multi-device connectivity.
- Build foundational knowledge in storage, networking, and ZFS.

## Hardware Summary
- **Base System:** Dell OptiPlex 3020
- **CPU:** Intel Core i5-4590 @ 3.30GHz
- **RAM:** Upgraded from 4GB to 8GB DDR3
- **Storage:** Replaced 500GB HDD with 2TB SATA drive
- **Add-ons:** PCIe Wi-Fi & Bluetooth card
- **Boot Device:** 32GB USB drive for TrueNAS SCALE OS

## OS and Software
- Upgraded from Windows 8.1 to Windows 11 (for hardware validation)
- Installed TrueNAS SCALE (25.04.1 Community Edition)
- Created SMB datasets: DocsShare, MediaShare, PhotoShare, jsanwo
- Static IP configured for persistent access
- Connected via CX File Explorer (Android) and Windows file explorer

## Current Status
The system is now running TrueNAS SCALE with shared datasets accessible over LAN. Remote access setup using Tailscale is pending and will be implemented in a follow-up project.

## Screenshots

![Web UI Dashboard](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/Web%20UI%20Dashboard.jpg)

![TueNas Core Installation before TrueNas Scale Installation](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/TueNas%20Core%20Installation%20before%20TrueNas%20Scale%20Installation.jpg)

![SMB Config](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/SMB%20Config.jpg)

![RAM Upgrade Before.](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/RAM%20Upgrade%20Before..jpg)

![RAM Upgrade After](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/RAM%20Upgrade%20After.jpg)

![PCIe Wifi Card](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/PCIe%20Wifi%20Card.jpg)

![Mapped Drive Window](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/Mapped%20Drive%20Window.jpg)

![HDD Installation In BIOS](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/HDD%20Installation%20In%20BIOS.jpg)

![Dataset Creation](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/Dataset%20Creation.jpg)

![CX File Access](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/CX%20File%20Access.jpg)

![BIOS Boot USB](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/BIOS%20Boot%20USB.jpg)

![Dataset Structure](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/Dataset%20Structure.jpg)

![smb share config](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/smb%20share%20config.jpg)

![Static IP settings](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/Static%20IP%20settings.jpg)

![User config ](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/User%20config%20.jpg)

![User Config shell](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade/blob/main/images/User%20Config%20shell.jpg)

---

## GitHub Repository Contents
- 📁 `images/` – Project snapshots & evidence of implementation
- 📄 `README.md` – This documentation

## Author
**Joseph Oladimeji Sanwo**  
📧 [LinkedIn](https://www.linkedin.com/in/jsanwo85/)  
🔗 [GitHub](https://github.com/jsanwo85)

## Tags
#TrueNAS #NAS #DellOptiPlex #OpenSource #ZFS #Networking #Cybersecurity #HomeLab
