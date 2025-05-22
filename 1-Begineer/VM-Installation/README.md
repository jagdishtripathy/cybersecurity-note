
# 🛡️ Installing Kali Linux on Windows (VMware & VirtualBox) -- Beginner's Guide

Welcome! This guide will help you install **Kali Linux** on **Windows** using two virtualization tools: **VMware Workstation Player** and **Oracle VirtualBox**. Whether you're new to cybersecurity or just starting with virtual machines, this step-by-step tutorial has you covered.

---

## 🧰 Prerequisites

- Windows 10/11 (64-bit)

- Minimum 4 GB RAM (8 GB recommended)

- At least 20 GB of free disk space

- Internet connection

---

## 🌀 OPTION 1: Installing Kali Linux with VMware Workstation Player

### ✅ Step 1: Download Required Tools

- **VMware Workstation Player (Free for personal use):**

  👉 [Download VMware](https://knowledge.broadcom.com/)

- **Kali Linux VMware Image (Prebuilt):**

  👉 [Download Kali Linux for VMware](https://www.kali.org/get-kali/#kali-virtual-machines)

  - Choose **"Kali Linux VMware 64-bit"**

  - File format: `.7z` (extract using [7-Zip](https://www.7-zip.org/))

### ✅ Step 2: Install VMware Workstation Player

1\. Run the downloaded `.exe` file.

2\. Follow the installation wizard and accept the license agreement.

3\. Launch VMware Player.

### ✅ Step 3: Import the Kali Linux VM

1\. Extract the `.7z` file using 7-Zip.

2\. Open VMware Workstation Player.

3\. Click **"Open a Virtual Machine"** and select the extracted `.vmx` file.

4\. Click **"Play Virtual Machine"** to start Kali Linux.

---

## 📦 OPTION 2: Installing Kali Linux with Oracle VirtualBox

### ✅ Step 1: Download Required Tools

- **Oracle VirtualBox:**

  👉 [Download VirtualBox](https://www.virtualbox.org/wiki/Downloads)

- **Kali Linux ISO File:**

  👉 [Download Kali ISO](https://www.kali.org/get-kali/#kali-installer-images)

  - Choose **Kali Linux 64-bit Installer ISO**

### ✅ Step 2: Install VirtualBox

1\. Run the VirtualBox `.exe` installer.

2\. Follow the setup instructions and install.

### ✅ Step 3: Create a New Virtual Machine

1\. Open VirtualBox and click **"New"**.

2\. Set the name to `Kali Linux`.

3\. Type: `Linux`, Version: `Debian (64-bit)`

4\. Allocate at least **2048 MB RAM** (4096 MB recommended).

5\. Create a new virtual hard disk (20 GB minimum).

6\. Select **VDI (VirtualBox Disk Image)** and **Dynamically allocated**.

### ✅ Step 4: Attach the Kali ISO & Start Installation

1\. Select the Kali VM and click **"Settings" > "Storage"**.

2\. Click the empty optical drive and choose the **Kali ISO**.

3\. Click **Start** to boot the VM and begin the installation.

### ✅ Step 5: Install Kali Linux

1\. Choose **"Graphical Install"**.

2\. Set your preferred language, location, and keyboard.

3\. Configure username, password, disk partitioning (select "Guided -- use entire disk").

4\. Finish installation and reboot.

---

## 🔐 Default Credentials

If using a **prebuilt image (VMware)**:

- **Username:** `kali`

- **Password:** `kali`

If installing manually:

- You'll set the username and password during setup.

---

## 💡 Useful Tips

- Always update your packages:

```
  sudo apt update && sudo apt upgrade
```
