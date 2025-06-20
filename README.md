# Upgrading and Repurposing a Dell OptiPlex 3020 into a Home NAS with TrueNAS SCALE

---

## 🧰 Overview

This hands-on home lab project demonstrates how I repurposed a legacy **Dell OptiPlex 3020** desktop to serve as a fully functional **Network Attached Storage (NAS)** system using **TrueNAS SCALE**.

The upgrade included hardware improvements, OS replacement, network tuning, and file-sharing configuration to transform the machine into a cost-effective personal cloud.

---

## 🎯 Objectives

- Extend the useful life of an old PC
- Learn hands-on server and storage configuration
- Build a low-cost home cloud solution
- Practice user permissions and ACL
- Prepare for remote access setup (still in progress)

---

## 🧱 Hardware Upgrades

| Component       | Before               | After                       |
|----------------|----------------------|-----------------------------|
| RAM            | 4GB DDR3             | 8GB DDR3 (2×4GB)            |
| Storage        | 500GB HDD            | 2TB SATA HDD                |
| Boot Device    | Internal HDD         | 32GB USB Stick (for OS)     |
| OS             | Windows 8            | Windows 11 → TrueNAS SCALE  |
| Networking     | None (no Wi-Fi)      | PCIe Wi-Fi & Bluetooth Card |
| Connectivity   | DHCP IP              | Static IP: 192.168.168.100  |

📸 _Photos below show before/after of RAM, storage, BIOS, and card installation._

---

## 💻 Software Configuration

### 🧩 Operating System
- **Upgraded from Windows 8 to Windows 11** for verification and backup
- Then, clean install of **TrueNAS SCALE** via bootable USB

### 🛠️ TrueNAS Setup
- Installed on external USB stick, 2TB HDD used as data pool (`Main`)
- Created datasets: `DocsShare`, `Main/jsanwo`
- Configured static IP address
- Setup SMB (Windows File Share) for LAN access

### 🔐 Permissions
- Created user: `jsanwo`
- Applied dataset ACL with full read/write permissions
- Connected from Android via **CX File Explorer** and Windows via mapped drive

---

## 🌐 Network Configuration

- Set router to assign **static IP** to TrueNAS: `192.168.168.100`
- Verified LAN access across devices
- 📱 Android + 🖥️ Windows both successfully connected to shared files

---

## 🐞 Challenges Faced

- `ix-applications` dataset permission issues
- ACL errors while saving user config
- SMB share mapping failures due to incorrect passwords
- Static IP reverting after reinstall
- ⚠️ **Tailscale and remote access app service** setup failed due to app deployment errors

> 🔧 **Remote access with Tailscale** is still a work in progress and will be handled as a follow-up project.

---

## 📸 Project Snapshots

> _Be sure your uploaded images are in the `/images/` folder for these to work properly._

### 🖼️ Hardware
- ![RAM Upgrade](images/ram_upgrade_after.jpg)
- ![HDD Installation](images/hdd_installation.jpg)
- ![PCIe Card](images/pcie_wifi_card.jpg)

### 🖥️ TrueNAS Setup
- ![BIOS Boot USB](images/bios_boot_usb.jpg)
- ![TrueNAS Web UI](images/web_ui_dashboard.jpg)
- ![Dataset Creation](images/dataset_creation.jpg)

### 🔄 Sharing
- ![SMB Access on Windows](images/mapped_drive_windows.jpg)
- ![CX File Access](images/cx_file_access.jpg)
- ![Router IP Reservation](images/router_static_ip.jpg)

---

## 📁 Config Files

All configuration notes can be found in the `/configs` folder:
- `dataset_structure.txt`
- `smb_share_config.yaml`
- `static_ip_settings.txt`

---

## ✅ Results

- Built a modern NAS from a 10-year-old machine
- Gained hands-on Linux & TrueNAS admin skills
- Successfully enabled LAN-based personal cloud
- 📌 Remote access setup (Tailscale) will be handled in **Phase 2**

---

## 🔗 Repository

All notes, configs, and screenshots are included in this repo.  
🔗 Shareable project link: `https://github.com/yourusername/dell-optiplex-truenas-upgrade`

---

## 💼 Tags

`#TrueNAS` `#ITProjects` `#HomeLab` `#Networking` `#Cybersecurity` `#OpenSource` `#DellOptiplex`

# Dell-optiplex-TrueNas-Upgrade
Repurposing a Dell OptiPlex 3020 into a Home NAS using TrueNAS SCALE
