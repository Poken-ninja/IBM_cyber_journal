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

✅ This version is structured, neat, and exam-ready.
Do you want me to also **add a flowchart/diagram** (like how user mode ↔ kernel mode communicate) for better presentation in your notes?
