# Upgrading and Repurposing a Dell OptiPlex 3020 into a Home NAS with TrueNAS SCALE

---

## Overview
In a hands-on home lab upgrade project, I repurposed a legacy Dell OptiPlex 3020 desktop to serve as a fully functional home Network Attached Storage (NAS) system. The process involved both hardware and software upgrades, including a transition from Windows 8 to Windows 11, increasing RAM, expanding storage, and implementing TrueNAS SCALE for data sharing and home network file management.

---

## Objectives
- Extend the life and capabilities of an old PC.
- Gain hands-on experience with NAS installation and configuration.
- Build a cost-effective private cloud storage solution.
- Enable file sharing and centralized data access across multiple devices on the same network.

---

## Hardware Upgrades
- **Base Machine:** Dell OptiPlex 3020 (BIOS firmware)
- **Original Specs:**
  - RAM: 4GB DDR3
  - HDD: 500GB
  - OS: Windows 8
- **Upgrades Performed:**
  - **RAM:** Upgraded from 4GB to 8GB DDR3 (by adding an extra 4GB module)
  - **Storage:** Replaced the 500GB HDD with a new 2TB SATA HDD
  - **Boot Device:** Installed TrueNAS SCALE on a 32GB USB flash drive
  - **Wireless Capability:** Installed a PCIe Wi-Fi and Bluetooth combo card
  - **Networking:** Connected system to LAN via Ethernet and Wi-Fi for admin access

---

## Software Configuration

### Operating System Upgrade
- Initially upgraded from Windows 8 to Windows 11 for validation and backup.
- Backed up data and proceeded with clean install of TrueNAS SCALE.

### TrueNAS SCALE Installation
- Booted from the prepared USB containing the TrueNAS SCALE ISO.
- Installed OS onto external USB while reserving 2TB drive as storage pool.
- Configured network settings for static IP.
- Created datasets for media and document storage (e.g., `DocsShare`, `Main/jsanwo`).
- Enabled SMB shares and tested access via CX File Explorer on Android and mapped drive on Windows.

### User and Permission Configuration
- Created dedicated user account `jsanwo` with proper ACLs and home directory.
- Granted user access to shared datasets with appropriate permissions.

---

## Network Configuration
- Configured the router to assign a **static IP** to the NAS device.
- Verified connectivity between NAS, smartphone (CX File Explorer), and Windows client.

---

## Challenges Faced
- Initial issues with `ix-applications` dataset permissions.
- Difficulty accessing the TrueNAS UI from Wi-Fi devices due to IP misalignment.
- Encountered errors with App Services preventing successful deployment of remote access solutions like Tailscale.
- Troubleshooting YAML deployment steps and resolving system permission constraints.

> ⚠️ **Note:** Remote access configuration using Tailscale is still a work in progress due to persistent App Service issues. This will be addressed in the next phase of the project.

---

## 📸 Screenshots

These images were captured throughout the process and show key steps in the upgrade and installation workflow.

| Description                     | Preview                                     |
|--------------------------------|---------------------------------------------|
| Web UI Dashboard               | ![](images/Web%20UI%20Dashboard.jpg)        |
| TrueNAS Core Installer         | ![](images/TueNas%20Core%20Installation%20before%20TrueNas%20Scale%20Installation.jpg) |
| SMB Shares                     | ![](images/SMB%20Config.jpg)                |
| RAM Before Upgrade             | ![](images/RAM%20Upgrade%20Before..jpg)     |
| RAM After Upgrade              | ![](images/RAM%20Upgrade%20After.jpg)       |
| PCIe WiFi Card Install         | ![](images/PCIe%20Wifi%20Card.jpg)          |
| Windows Network Map            | ![](images/Mapped%20Drive%20Window.jpg)     |
| HDD in BIOS                    | ![](images/HDD%20Installation%20In%20BIOS.jpg) |
| Dataset Creation               | ![](images/Dataset%20Creation.jpg)          |
| CX File Explorer (Mobile Access) | ![](images/CX%20File%20Access.jpg)       |
| BIOS Boot Order                | ![](images/BIOS%20Boot%20USB.jpg)           |
| Storage Status on TrueNAS      | ![](images/Dataset%20Structure.jpg)         |
| SMB Share Config Edit View     | ![](images/smb%20share%20config.jpg)        |
| Static IP Settings             | ![](images/Static%20IP%20settings.jpg)      |
| User Configuration (Edit)      | ![](images/User%20config%20.jpg)           |
| User Shell Details             | ![](images/User%20Config%20shell.jpg)       |

---

## Outcome & Impact
- Successfully transformed a non-critical, outdated desktop into a modern, secure NAS.
- Built foundational skills in ZFS, dataset permissions, and SMB sharing.
- Enabled secure file access across multiple LAN devices (remote access pending).

---

## Repository and Documentation  
📂 [GitHub Project Repo](https://github.com/jsanwo85/Dell-optiplex-TrueNas-Upgrade)

---

## Conclusion
This project demonstrates how an obsolete PC can be converted into a valuable asset for personal cloud storage using open-source technologies. It offers a strong introduction into enterprise-level storage concepts at home and is a worthwhile showcase for IT and cybersecurity professionals. The remote access component using Tailscale will follow as a standalone project in the next iteration.

---

## Author  
**Joseph Oladimeji Sanwo**  
📧 joseph.sanwo1@gmail.com

---

**Tags:** `#TrueNAS` `#HomeLab` `#NAS` `#ITProjects` `#Cybersecurity` `#DellOptiPlex` `#OpenSource` `#Storage` `#Networking`
