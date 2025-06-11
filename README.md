# EasySave – Backup Software

**EasySave** is a modular and scalable backup software developed in C# (.NET 8.0) as part of the ProSoft suite. It enables users to automate file backups, monitor their progress in real time, and ensure data security through configurable options and encryption. The software evolves across multiple versions, each introducing new functionalities and improvements.

---

## 🧩 Project Summary

EasySave was developed in three main stages:

### 🔹 Version 1.0 – Console Application
- Supports up to 5 backup jobs
- Manual or sequential execution
- Backup types: Full or Differential
- Real-time logs in JSON format
- State tracking file for live progress monitoring
- Executable via command line (e.g., `dotnet run -- 1-3`)

### 🔹 Version 1.1 – Extended Logging
- Same as v1.0 with added support for **XML** logging
- Users can choose between **JSON** or **XML** log formats
- Maintains compatibility with v1.0 features

### 🔹 Version 2.0 – Graphical User Interface (WPF)
- Modern UI with unlimited backup jobs
- Integration with external encryption tool **CryptoSoft**
- Optional file encryption based on file extensions
- Logging includes encryption time
- Detection of business applications (e.g., calculator)
  - If detected, backup is blocked
- Real-time progress display in GUI

### 🔹 Version 3.0 – Parallel Execution & Remote Control
- **Parallel backup execution**
- **Priority file handling**: priority extensions are backed up first
- Restricts simultaneous transfer of large files (user-defined size)
- Detects business software in real-time:
  - Pauses all jobs until software closes
- **Remote monitoring GUI** using **Sockets**
- User control: Pause, Resume, Stop for each job
- CryptoSoft runs as a **mono-instance**

---

## ⚙️ Core Features

- 🔄 **Full / Differential backup support**
- 📂 **Local, external, or network drive compatibility**
- 🌐 **Multilingual**: English and French
- 📊 **Log files**: JSON and/or XML (readable format)
- 🔐 **File encryption**: via CryptoSoft (v2.0+)
- ⏱️ **Real-time state tracking**
- 🖥️ **WPF UI (v2.0+)** and **Remote Console (v3.0)**
- ⚠️ **Business software awareness**: to avoid resource conflicts

---

