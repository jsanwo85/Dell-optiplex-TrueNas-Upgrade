# 🛠️ Dell OptiPlex 3020 → TrueNAS SCALE Upgrade Project

## Overview

This project demonstrates how I repurposed an aging **Dell OptiPlex 3020** desktop into a fully functional home **NAS server** using **TrueNAS SCALE**. The upgrade involved increasing hardware capacity, switching from Windows 8.1 to 11 for testing, and finally installing TrueNAS SCALE as the operating system to manage shared storage over my LAN.

---

## Objectives

- Upgrade legacy hardware to extend its lifespan.
- Learn and deploy a functional home NAS using open-source software.
- Host shared storage over local network with SMB and access via mobile and desktop.
- Document the setup to showcase real-world IT support and system administration skills.

---

## Hardware Upgrade Summary

| Component      | Original                     | Upgraded                          |
|----------------|------------------------------|------------------------------------|
| RAM            | 4GB DDR3                     | 8GB DDR3 (added extra 4GB)        |
| Storage        | 500GB HDD                   | 2TB Seagate SATA HDD              |
| OS             | Windows 8.1 Pro             | Upgraded briefly to Windows 11    |
| Network        | No Wi-Fi                    | PCIe Wi-Fi + Bluetooth combo card |
| Boot Device    | Internal HDD                | 32GB USB drive with TrueNAS SCALE |

---

## Software & Configuration

- Flashed TrueNAS SCALE ISO to USB using Rufus
- Installed to a second USB drive; dedicated 2TB drive for storage pool
- Created multiple datasets: `Document`, `Media`, `Photo`, `jsanwo`
- Enabled SMB for all datasets
- Created a user (`jsanwo`) with proper access and ACLs
- Configured static IP: `192.168.168.100`
- Verified access via Windows and Android using CX File Explorer

---

## Challenges

- App Services failing to install apps like Tailscale due to permission errors in `ix-applications`
- CLI permission issues as root access is restricted in TrueNAS SCALE Web UI
- Sharing externally still **in progress** (will be tackled in a separate project)

---

## Screenshots

> These images were captured throughout the process and show key steps in the upgrade and installation workflow.

| Description                         | Preview                                                   |
|-------------------------------------|------------------------------------------------------------|
| Web UI Dashboard                    | ![](images/Web%20UI%20Dashboard.jpg)                      |
| TrueNAS Core Installer              | ![](images/TueNas%20Core%20Installation%20before%20TrueNas%20Scale%20Installation.jpg) |
| SMB Shares                          | ![](images/SMB%20Config.jpg)                              |
| RAM Before Upgrade                  | ![](images/RAM%20Upgrade%20Before..jpg)                   |
| RAM After Upgrade                   | ![](images/RAM%20Upgrade%20After.jpg)                     |
| PCIe WiFi Card Install              | ![](images/PCIe%20Wifi%20Card.jpg)                        |
| Windows Network Map                 | ![](images/Mapped%20Drive%20Window.jpg)                   |
| HDD in BIOS                         | ![](images/HDD%20Installation%20In%20BIOS.jpg)            |
| Dataset Creation                    | ![](images/Dataset%20Creation.jpg)                        |
| CX File Explorer (Mobile Access)    | ![](images/CX%20File%20Access.jpg)                        |
| BIOS Boot Order                     | ![](images/BIOS%20Boot%20USB.jpg)                         |
| Storage Pool on TrueNAS            | ![](images/Dataset%20Structure.jpg)                       |
| SMB Share Config                    | ![](images/smb%20share%20config.jpg)                      |
| Static IP Config                    | ![](images/Static%20IP%20settings.jpg)                    |
| User Setup                          | ![](images/User%20config%20.jpg)                          |
| User Shell Permissions              | ![](images/User%20Config%20shell.jpg)                     |

---

## Outcome

✅ Local storage working  
✅ Accessible from both Android and Windows  
🚧 Remote access via Tailscale still in progress  
📌 Valuable hands-on experience with NAS, datasets, ACL, SMB, BIOS, and system installation

---

## GitHub Repository

- Project Page: [https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade)

---

## Tags

`#TrueNAS` `#DellOptiplex3020` `#NAS` `#SMB` `#ZFS` `#CXFileExplorer` `#CybersecurityProjects` `#OpenSource` `#WindowsToLinux`

---

## Author

**Joseph Oladimeji Sanwo**  
MSc Applied Cybersecurity – UK  
Email: lizteevera@gmail.com  
GitHub: [@jsanwo85](https://github.com/jsanwo85)

---

## License

This documentation is released under the [MIT License](LICENSE).
