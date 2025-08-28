# **Windows 10 Overview**

Windows 10 is a versatile operating system (OS) designed for desktops, laptops, and mobile devices. It regularly receives **updates** for new features, security, and performance improvements.

---

## **File Systems in Windows**

File systems provide the foundation for accessing, storing, and organizing files.

* **FAT (File Allocation Table):**
  Older system, simple but limited in scalability.

* **NTFS (New Technology File System):**
  Advanced system used in modern Windows, supports **security, permissions, compression, and large files**.

**Metadata** (size, permissions, timestamps) maintains **data integrity**.

---

## **Windows File Organization**

Windows uses a **hierarchical (tree-like) structure**.

* **Root directory:** `C:\`
* **Key folders:**

  * `Users` → personal profiles, documents, downloads.
  * `Windows` → system files.
  * **System32** → essential 32-bit system files.
  * **SysWOW64** → support for 32-bit applications on 64-bit systems.

➡️ Separation of 32-bit and 64-bit files ensures compatibility and stability.

---

## **32-bit vs 64-bit Systems**

* **32-bit systems:**

  * Can address up to **4 GB memory** only.
  * Struggle with modern software.

* **64-bit systems:**

  * Can use **large amounts of memory**.
  * Faster performance with **big data and heavy applications**.

---

## **Processor Modes in Windows**

Windows processors work in **two modes**:

1. **User Mode**

   * Applications run here.
   * Each process has a **separate virtual address space**.
   * Crashes usually affect only the application, not the OS.

2. **Kernel Mode**

   * Core of the OS, device drivers, and system services.
   * **All processes share the same address space.**
   * A crash here can bring down the entire system (Blue Screen).

➡️ **System Calls** act as the bridge between **user mode and kernel mode**.

---

## **Hands-on Learning**

Microsoft offers **Windows Lab Workspace**, a virtual practice environment to experiment with Windows concepts and commands safely.

---

# **Windows Command Prompt Tools for Administration**

The **CMD (Command Line Interface)** in Windows allows administrators to manage, configure, and troubleshoot the system using text-based commands.

---

## **1. Group Policy Management**

* **gpupdate** → Refresh/apply Group Policy immediately.
  *Options:* `/target:user` (user policies), `/target:computer` (computer policies).
* **gpresult** → Show applied policies for user or computer.
  *Options:* `/r` (summary), `/v` (detailed/verbose).

---

## **2. Drive Letters & File Navigation**

* **vol \[drive:]** → Display drive volume info (label, serial number, file system).
* **chdir (cd)** → Change directory. Example: `cd D:` switches to D drive.
* **cd \[folder]** → Navigate inside current drive (e.g., `cd Documents`).

---

## **3. System Maintenance & Info**

* **shutdown** → Shutdown/restart with options (`/s`, `/r`, `/t`).
* **sfc /scannow** → Scan & repair corrupted system files.
* **chkdsk \[drive:]** → Check & fix disk errors, bad sectors.
* **diskpart** → Partition manager (create, delete, resize partitions).
* **winver** → Show Windows version & build info.
* **format \[drive:] /FS\:NTFS (or FAT32)** → Format disk with specified file system.

---

## **4. Managing Files & Directories**

* **dir** → List files/folders in current directory.
* **md \[name]** → Make new directory.
* **rd \[name]** → Remove directory (`/s` for recursive deletion).
* **ren \[old] \[new]** → Rename file/folder.
* **del \[file]** → Delete file(s), e.g., `del *.txt` deletes all text files.

---

## **5. File Copying & Backup**

* **copy \[src] \[dest]** → Copy single/multiple files.
  *Options:* `/v` verify, `/y` overwrite silently.
* **xcopy \[src] \[dest] /s /e** → Advanced copy (includes subdirs & empty folders).
* **robocopy \[src] \[dest] /MIR** → Robust copy (mirroring, retrying, multi-threading).

---

## **6. Hostname & Network Tools**

* **hostname** → Display computer’s hostname.
* **ipconfig** → Show IP address, subnet mask, gateway, DNS.
* **ping \[host/IP]** → Test network connectivity & measure latency.

---

✅ **Summary:**

* Group Policy → `gpupdate`, `gpresult`
* Drive Letters → `vol`, `cd`, `chdir`
* System Maintenance → `shutdown`, `sfc`, `chkdsk`, `diskpart`, `winver`, `format`
* Files/Directories → `dir`, `md`, `rd`, `ren`, `del`
* File Copying → `copy`, `xcopy`, `robocopy`
* Networking → `hostname`, `ipconfig`, `ping`

---

