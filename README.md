# Kali-Setup
My personal Kali Linux setup — installation steps, VM config, essential tools, aliases, and tweaks for Red Team operations.

# Kali-Setup (Windows Host)
Personal Kali Linux setup for Red Team training using a **Windows machine as the host**.  
Includes VM installation, configuration, post-install tweaks, and essential pentesting tools.

---

## 🖥️ Host Environment

- **Host OS**: Windows 10/11  
- **Virtualization**: VirtualBox or VMware  
- **Target Guest**: Kali Linux (Debian-based)

---

## 📦 System Requirements

- CPU with virtualization enabled (Intel VT-x / AMD-V)
- 8 GB RAM (16 GB recommended)
- 40 GB free SSD storage (recommended)
- VirtualBox or VMware installed
- Internet connection

**Check if virtualization is enabled:**

- Task Manager > Performance > CPU → "Virtualization: Enabled"  
- Or run in CMD:

- ![image](https://github.com/user-attachments/assets/793f00db-e1d9-419b-a008-ee0904dacd05)

- ---

## 🔗 Official Downloads (Windows Host)

### 1. Kali Linux ISO
Download the latest Kali Linux installer ISO (64-bit) from the official website:

- 🌐 Website: [https://www.kali.org/get-kali/](https://www.kali.org/get-kali/)
![image](https://github.com/user-attachments/assets/1e81f885-6e44-4494-8577-03d963a7a812)


- 📥 Direct ISO Link:  
  (https://www.kali.org/get-kali/#kali-installer-images)

  ![image](https://github.com/user-attachments/assets/3d4be01f-2d50-49f0-b495-f83d6358d868)

  

> Recommended: Use the **Installer ISO** (not the live version) for better compatibility and updates.

---

### 2. VirtualBox (Recommended)

If you don’t have a virtualization tool installed, download **VirtualBox**:

- 🌐 Website: [https://www.virtualbox.org/wiki/Downloads](https://www.virtualbox.org/wiki/Downloads)
- 📥 Direct Windows EXE:  
  [[https://download.virtualbox.org/virtualbox/7.0.18/VirtualBox-7.0.18-162988-Win.exe](https://cdimage.kali.org/kali-2025.2/kali-linux-2025.2-installer-amd64.iso)]([https://download.virtualbox.org/virtualbox/7.0.18/VirtualBox-7.0.18-162988-Win.exe](https://cdimage.kali.org/kali-2025.2/kali-linux-2025.2-installer-amd64.iso))

💡 Optional: Download the **VirtualBox Extension Pack** (adds USB 3.0, drag-drop, shared clipboard):
- 📦 [https://download.virtualbox.org/virtualbox/7.0.18/Oracle_VM_VirtualBox_Extension_Pack-7.0.18.vbox-extpack](https://download.virtualbox.org/virtualbox/7.0.18/Oracle_VM_VirtualBox_Extension_Pack-7.0.18.vbox-extpack)

---


