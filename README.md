# 🎓 Twiby v1.2: Automated Student Orientation Twibbon Engine

[![Release](https://img.shields.io/badge/Release-v1.2.0--stable-blue.svg)](#)
[![Platform](https://img.shields.io/badge/Platform-Windows%20x64-brightgreen.svg)](#)
[![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)](#)

Twiby is a lightweight desktop application designed to automate official student orientation frame generation. It eliminates the need for manual photo editing software by automatically aligning orientation templates, adjusting color channels, and packaging your final submission assets.

Twiby includes both an interactive Graphical User Interface (GUI) and a Command Line Interface (CLI).

---

## [1] Usage Instructions

### Option 1: Graphical User Interface (GUI)

1. Double-click `twiby.exe` to launch the application window.
2. Click the **Browse...** button to select your profile picture.
3. Click **Apply Twibbon Frame**.
4. The processed asset will be generated in the same directory as your selected image with an added `.enc` extension (e.g., `me.png.enc`).

### Option 2: Command Line Interface (CLI)

You can also run Twiby directly from Command Prompt or PowerShell:

```cmd
twiby.exe -i "me.png"

```

To process an image from another folder or drive, pass the absolute path:

```cmd
twiby.exe -i "D:\Photos\Orientation\student_profile.jpg"

```

---

## [2] Requirements and Format Validation

* **Operating System:** Windows 10 / 11 (64-bit)
* **Supported Formats:** PNG, JPG, JPEG
* **Validation:** Twiby inspects the binary image header to ensure file integrity. Renaming an invalid file extension will cause processing to abort.
* **Dependencies:** Standalone executable. No additional runtimes required.

---

## [3] Notes and Troubleshooting

* **Source File Handling:**
To optimize storage during batch generation, Twiby clears the temporary source image buffer once the protected output container is written. Always keep a backup copy of your original photo before running the tool.
* For system validation errors or corrupt image headers, verify your original photo and try again.

---
```py
print("Happy Oriented")
