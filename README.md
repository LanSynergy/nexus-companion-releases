# Nexus Companion — Official Desktop Releases

Welcome to the official distribution repository for **Nexus Companion**, the agent-native research workspace.

Nexus Companion provides an offline-capable, local-first research environment equipped with 138 domain-specific research tools, DuckDB dataset analytics, native Word/Excel/PowerPoint document authoring (`officecli`), systematic academic literature review engines (PubMed, arXiv, CrossRef), and 100% local confinement.

---

## 📥 Downloads (Latest Release)

| Platform | Package Type | Direct Download Link |
|---|---|---|
| **Windows** | Standalone Installer (`.exe`) | [Download `nexus-desktop-windows-x64.exe`](https://github.com/LanSynergy/nexus-companion-releases/releases/latest/download/nexus-desktop-windows-x64.exe) |
| **Windows** | Portable Archive (`.zip`) | [Download `nexus-desktop-windows-x64.zip`](https://github.com/LanSynergy/nexus-companion-releases/releases/latest/download/nexus-desktop-windows-x64.zip) |
| **Linux** | AppImage (`.AppImage`) | [Download `nexus-desktop-linux-x86_64.AppImage`](https://github.com/LanSynergy/nexus-companion-releases/releases/latest/download/nexus-desktop-linux-x86_64.AppImage) |
| **Linux** | Compressed Archive (`.tar.gz`) | [Download `nexus-desktop-linux-x86_64.tar.gz`](https://github.com/LanSynergy/nexus-companion-releases/releases/latest/download/nexus-desktop-linux-x86_64.tar.gz) |
| **Linux** | Standalone Binary | [Download `nexus-desktop-linux-x86_64`](https://github.com/LanSynergy/nexus-companion-releases/releases/latest/download/nexus-desktop-linux-x86_64) |

*All releases and historical tags are accessible on the [Releases Page](https://github.com/LanSynergy/nexus-companion-releases/releases).*

---

## 💻 Windows Installation & Setup Guide

Nexus Companion for Windows runs natively on 64-bit Windows 10 and Windows 11.

### 1. Running the `.exe` Installer
1. Download **[`nexus-desktop-windows-x64.exe`](https://github.com/LanSynergy/nexus-companion-releases/releases/latest/download/nexus-desktop-windows-x64.exe)**.
2. Double-click the downloaded file to launch the application.

### 🛡️ Windows SmartScreen Notice (Important)
Because this is an early preview beta release, the executable has not yet been signed with a commercial certificate. Windows Defender SmartScreen may display a blue warning box stating:
> *"Windows protected your PC — Microsoft Defender SmartScreen prevented an unrecognized app from starting."*

To continue launching:
1. Click the **"More info"** text link on the dialog.
2. Click the **"Run anyway"** button that appears in the bottom right corner.
3. Nexus Companion will launch and initialize your local research workspace.

---

### 2. Using the Portable `.zip`
If you prefer not to use an installer:
1. Download **[`nexus-desktop-windows-x64.zip`](https://github.com/LanSynergy/nexus-companion-releases/releases/latest/download/nexus-desktop-windows-x64.zip)**.
2. Right-click the `.zip` file and select **Extract All...**.
3. Open the extracted folder and run **`nexus-desktop.exe`** directly.

---

## 🐧 Linux Installation & Setup Guide

Nexus Companion is distributed for x86_64 Linux systems (Ubuntu, Debian, Fedora, Arch, and derivatives).

### 1. Running the AppImage (Recommended)
1. Download **[`nexus-desktop-linux-x86_64.AppImage`](https://github.com/LanSynergy/nexus-companion-releases/releases/latest/download/nexus-desktop-linux-x86_64.AppImage)**.
2. Make the file executable and run it:
   ```bash
   chmod +x nexus-desktop-linux-x86_64.AppImage
   ./nexus-desktop-linux-x86_64.AppImage
   ```

> **Note for Ubuntu 22.04+ / Debian users**: If your system does not have FUSE installed, install `libfuse2`:
> ```bash
> sudo apt install libfuse2
> ```

---

### 2. Extracting the `.tar.gz` Archive
1. Download **[`nexus-desktop-linux-x86_64.tar.gz`](https://github.com/LanSynergy/nexus-companion-releases/releases/latest/download/nexus-desktop-linux-x86_64.tar.gz)**.
2. Extract and launch:
   ```bash
   tar -xzf nexus-desktop-linux-x86_64.tar.gz
   ./nexus-desktop-linux-x86_64
   ```


## 🔒 Security & Confinement

- **Local Execution**: All LLM interactions, research tools, dataset operations, and document generation execute 100% locally on your machine.
- **Sandboxed Subprocesses**: Commands and scripts run confined to your chosen research workspace directory using OS-native sandbox backends (Bubblewrap on Linux, restricted security tokens on Windows).
