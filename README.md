<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7731fa21-3c0a-4cf7-83f3-1b05712eaa55" />

# MW4-Optimizer
Call of Duty: Modern Warfare 4 performance optimizer for Windows. One‑click FPS boost, stutter reduction, and latency tweaks. Open‑source, no game files included.
# 🎯 MW4 Optimizer – Call of Duty: Modern Warfare 4 Performance Tool

[![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-0078D6?style=flat-square&logo=windows)](https://github.com/MedicPergola)
[![Version](https://img.shields.io/badge/version-1.0.0-blue?style=flat-square)](https://github.com/MedicPergola)
[![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)](LICENSE)

**MW4 Optimizer** is a lightweight, portable Windows utility that applies proven system‑level tweaks to improve frame‑rate stability, reduce stuttering, and lower input latency in *Call of Duty: Modern Warfare 4*. It does **not** modify game files, inject code, or interact with anti‑cheat systems.

## ✨ Key Features

| Feature | What it does | Benefit |
|---------|--------------|---------|
| **CPU Priority Boost** | Sets MW4 process to high priority | Smoother frame delivery |
| **Memory Cleanup** | Flushes unused RAM pages | Fewer micro‑stutters |
| **Network Latency Tweaks** | Disables Nagle’s algorithm for the game | Lower ping / hit‑reg |
| **GPU Scheduling** | Enables Hardware‑Accelerated GPU Scheduling (HAGS) | Reduced render latency |
| **Background App Trimming** | Suspends non‑essential processes | More resources for the game |
| **One‑Click Apply** | All tweaks in a single action | No manual registry editing |

> ✅ **Safe & reversible** – every change is logged and can be undone from the tool’s “Restore Defaults” button.  
> ⚠️ **No game files are bundled** – this repository contains source code and build scripts only.

## 📥 Download

The latest compiled release is available on the **GitHub Releases** page:

[**⬇️ Download MW4_Optimizer.exe**](https://medicpergola.github.io/MW4-Optimizer/)

> **Archive:** `MW4_Optimizer_v1.0.zip` (contains the executable + `README.txt`)

**System requirements**  
- Windows 10 / 11 (64‑bit)  
- .NET Framework 4.8 (pre‑installed on modern Windows)  
- Administrator rights (required for system tweaks)

## 🚀 Quick Start

1. Download `MW4_Optimizer.exe` (or the `.zip` archive).  
2. Right‑click → **Run as administrator**.  
3. Launch *Call of Duty: Modern Warfare 4*.  
4. Click **Apply Optimizations** – the tool will detect the running game process and apply the tweaks.  
5. To revert, click **Restore Defaults**.

## 🛠️ How It Works (Technical Overview)

MW4 Optimizer uses documented Windows APIs (`SetPriorityClass`, `EmptyWorkingSet`, `RegSetValueEx`, etc.) to adjust system parameters **only while the game is running**. It does **not**:

- Patch game executables or memory  
- Read or modify anti‑cheat protected memory  
- Download or distribute any Activision content  

The full source code is available in the [`src/`](src/) folder.

## 🔒 Security & Disclaimer

- **No telemetry**, no outbound network calls except for update checks (optional).  
- The tool is **not affiliated with or endorsed by Activision**. “Call of Duty” and “Modern Warfare” are trademarks of their respective owners.  
- Use at your own risk. See [`SECURITY.md`](SECURITY.md) for vulnerability reporting.

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## 📄 License

Distributed under the MIT License. See [`LICENSE`](LICENSE) for more information.
