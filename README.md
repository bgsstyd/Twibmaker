# 🎓 TwibMaker v1.2 Automated Student Orientation Twibbon Engine

[![Release](https://img.shields.io/badge/Release-v1.2.0--stable-blue.svg)](#)
[![Python 3.10+](https://img.shields.io/badge/Python-3.10+-yellow.svg)](#)
[![Platform](https://img.shields.io/badge/Platform-Windows%20x64-brightgreen.svg)](#)
[![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)](#)

An automated lightweight desktop utility engineered to streamline the profile frame generation process for the **2026 Student Orientation & School Induction Week (MPLS)**. No graphic editing tools (Photoshop/Canva) required.

The engine automatically processes aspect-ratio adjustments, optimizes rendering resolution, and aligns the official orientation frame directly onto your submitted photo asset.

---

## 📌 Usage Instructions

1. **Download Executable:**
   * Download the latest `twibmaker.exe` binary from the [Releases](../../releases) section or from the official distribution channel.
2. **Stage Your Photo:**
   * Place your orientation photo into the exact same folder as `twibmaker.exe`.
   * **IMPORTANT:** Rename your image file to `flag.png` (must be a valid `.png` file).
3. **Execute the Generator:**
   * Double-click `twibmaker.exe`.
   * The pipeline will initialize the asset rendering stream, apply the orientation frame template, and encapsulate the image container.
4. **Output:**
   * Once rendering concludes, your optimized asset will be compiled into `flag.png.enc`, formatted and ready for submission to the school verification portal.

---

## 🛠️ System Requirements

* **Operating System:** Windows 10 / 11 (64-bit)
* **Supported File Format:** Portable Network Graphics (`.png`)
* **Dependencies:** None *(Self-contained standalone binary)*

---

## ⚙️ Building from Source

For IT staff and student committee leads compiling from source:

```bash
# Clone the repository
git clone [https://github.com/orientation-committee-2026/TwibMaker-Engine.git](https://github.com/orientation-committee-2026/TwibMaker-Engine.git)
cd TwibMaker-Engine

# Install required dependencies
pip install -r requirements.txt

# Run the pipeline directly
python twibmaker.py
