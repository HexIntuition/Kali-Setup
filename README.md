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
 ![image](https://github.com/user-attachments/assets/49b61c8b-0a28-416c-b720-6748aab772f7)


---

## 💻 Virtual Machine Setup (Step-by-Step)

Now that VirtualBox is installed and ready (see image below), let’s create the Kali Linux VM from scratch.

![image](https://github.com/user-attachments/assets/66ccb115-40db-4bd1-b8ea-568931ca9ff0)



---

### ✅ Step 1: Create a New Virtual Machine

1. Click the green `New` button in the top menu.
   ![image](https://github.com/user-attachments/assets/59367b3b-c424-4861-9ac3-75cf70a6daf6)

2. Name your VM (e.g., `Kali-RedTeam`).
   ![image](https://github.com/user-attachments/assets/b3f5aaf0-c563-4a5b-b7dc-13f4f8a4dcda)

3. Choose:
   - **Type**: Linux
   - **Version**: Debian (64-bit)
     ![image](https://github.com/user-attachments/assets/4f669566-8cb2-4daf-b758-c815b016fd0f)

4. Click **Next**.

---

### ✅ Step 2: Allocate Memory (RAM)

- Minimum: 4096 MB (4 GB)
      ![image](https://github.com/user-attachments/assets/88750399-1ff7-4da5-aaaf-0346e64da6f4)


- Recommended: 8192 MB (8 GB) or more if available

---

### ✅ Step 3: Create a Virtual Hard Disk

- Select: `Create a virtual hard disk now`
- Choose:
   - **Size**: At least 40 GB (SSD recommended)
     ![image](https://github.com/user-attachments/assets/a89d3eec-4258-49b9-8984-2f43499e7209)


Click **finish** to finish.
![image](https://github.com/user-attachments/assets/b726e445-b06b-4712-a0d7-4abf39887b96)


---

### ✅ Step 4: Attach the Kali Linux ISO

1. Select your new VM > click **Settings**
   ![image](https://github.com/user-attachments/assets/4aaf8be8-e039-4161-93f9-b98cfa3a803d)

2. Go to **Storage** tab
   ![image](https://github.com/user-attachments/assets/ff8ea5bc-d881-4f46-8e59-fb0fb96d901d)

3. Click the **Empty optical drive**, then click the **disc icon** on the right → Choose a disk file
   ![image](https://github.com/user-attachments/assets/1355edee-de32-4a35-a17e-fd29d52f0206)

4. Select your Kali Linux ISO (downloaded earlier)
   ![image](https://github.com/user-attachments/assets/39f5f520-7dc5-48b1-b669-5a4c269ef7a7)

5. Click OK
   ![image](https://github.com/user-attachments/assets/19587969-305d-468d-a25a-3a4b68966763)

Your Kali ISO is now mounted and ready to boot.

---

### ✅ Step 5: Network Setup (Optional but recommended)

- Go to **Settings > Network**
- Adapter 1 → Attached to: `Bridged Adapter` or leave it as `NAT` for now
  ![image](https://github.com/user-attachments/assets/b0f8d944-6357-4837-b714-56961cf6a849)

- Bridged gives you a real IP in the same network (useful later for network tools)

---

### ✅ Step 6: Start the Machine

- Select your VM → click **Start**
  ![image](https://github.com/user-attachments/assets/fe99f3e2-86fa-4ff4-bea3-fdff9df70901)

- The Kali installer should launch
- Choose: `Graphical Install`
  ![image](https://github.com/user-attachments/assets/5c2aeb38-49f8-4e90-93b2-cd4e5bd05c04)


Now you're inside the Kali Linux installation process. 🎉

---

> 🧠 Tip: This part might feel "basic", but it's where most people stop. If you made it this far, you're already past the hesitation barrier.

Next section: **Installing Kali step-by-step inside the VM**.




