# PasswordToolbox 🛡️

<div align="center">

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![.NET](https://img.shields.io/badge/.NET-8.0-purple.svg)
![Platform](https://img.shields.io/badge/platform-Windows-yellow.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)

</div>

> A powerful Windows desktop application with 20+ security and encoding tools for developers and security-conscious users.

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [How to Use](#-how-to-use)
- [Requirements](#-requirements)
- [Installation](#-installation)
- [Build from Source](#-build-from-source)
- [Security Notes](#-security-notes)
- [License](#-license)

## ✨ Overview

PasswordToolbox is a WPF desktop application that provides essential security and encoding utilities in one convenient place. All tools run locally on your machine - no data is sent to external servers.

## 🎯 Features

### 🔐 Security Tools

| Tool | Description | How to Use |
|------|-------------|-------------|
| **Disk & USB password** | Open BitLocker, VeraCrypt settings | Click to launch Windows encryption settings |
| **Encrypt file** | AES-GCM encryption (max 512 MB) | Select file → Enter password → Save encrypted .pbxenc |
| **Password-protect folder** | ZIP with AES-256 | Select folder → Set password → Creates protected ZIP |
| **Folder hide** | CLSID style folder hiding | Select folder → Password protects visibility |
| **Password generator** | Cryptographically random | Configure length, chars → Copy generated password |
| **Password strength check** | Local heuristic analysis | Enter password → See strength score |

### 🔑 Secrets Tools

| Tool | Description | How to Use |
|------|-------------|-------------|
| **Random bytes** | Secure random hex | Set bytes count → Generate → Copy |
| **UUID/GUID** | Version 4 generators | Click generate → Copy UUID |

### 🔤 Encoding Tools

| Tool | Description | How to Use |
|------|-------------|-------------|
| **Base64** | Encode/decode UTF-8 | Enter text → Encode/Decode → Copy result |
| **URL encode** | Percent-encoding UTF-8 | Enter text → Encode/Decode |
| **JWT decode** | Pretty-print header & payload | Paste JWT → See decoded JSON |
| **JSON format** | Pretty-print and minify | Paste JSON → Format/Minify |
| **Unix time** | Epoch ↔ date conversion | Enter timestamp → See date & vice versa |

### 📁 Files Tools

| Tool | Description | How to Use |
|------|-------------|-------------|
| **File hashes** | SHA-256, SHA-1, MD5 | Drop/select file → Copy hash |
| **Text hashes** | SHA-256, SHA-1, MD5 | Enter text → See all hashes |
| **QR code** | Generate PNG QR codes | Enter text → Generate → Copy to clipboard |

### 🔒 Privacy & Diagnostics Tools

| Tool | Description | How to Use |
|------|-------------|-------------|
| **Clear clipboard** | Wipe clipboard immediately | Click to clear |
| **System info** | OS and runtime details | View system information |
| **USB security tips** | BitLocker, VeraCrypt guide | Read security recommendations |

## 🚀 How to Use

1. **Launch the app** - Run `PasswordToolbox.exe`
2. **Browse tools** - Use the search bar or scroll through categories
3. **Select a tool** - Click on any tool to open it
4. **Use the tool** - Follow on-screen instructions for each tool

### Searching for Tools
- Type in the search box to filter tools by name, description, or category
- The counter shows filtered/total tools

### Tool Categories
- **Security** 🔐 - Encryption, passwords, disk protection
- **Secrets** 🔑 - Random generators, UUIDs
- **Encoding** 🔤 - Text encoding/decoding utilities
- **Files** 📁 - File processing, hashing, QR codes
- **Privacy** 🔒 - Clipboard, system info, guides
- **Roadmap** 📋 - Planned future features

## ⚙️ Requirements

- **Operating System**: Windows 10 or Windows 11
- **Runtime**: .NET 8.0 Desktop Runtime
- **RAM**: 100 MB minimum
- **Disk**: 50 MB for installation

## 📥 Installation

### Option 1: Pre-built Release
1. Download the latest release from the Releases page
2. Extract the ZIP file
3. Run `PasswordToolbox.exe`

### Option 2: Install .NET Runtime
If you don't have .NET 8.0 Runtime:
1. Download from [Microsoft](https://dotnet.microsoft.com/download/dotnet/8.0)
2. Run the installer
3. Launch PasswordToolbox

## 🔨 Build from Source

```bash
# Clone the repository
git clone https://github.com/yourusername/PasswordToolbox.git
cd PasswordToolbox

# Build and run
dotnet run --project PasswordToolbox/PasswordToolbox.csproj
```

## 🔒 Security Notes

- ✅ All encryption happens locally on your device
- ✅ No data is sent to external servers
- ✅ Passwords are never stored (except for folder protection which uses a local hash)
- ⚠️ For sensitive data, always use strong passwords
- ⚠️ Backup your encrypted files

## 🛠️ Tech Stack

- **Framework**: .NET 8.0 / WPF
- **UI**: XAML with custom styling
- **Libraries**:
  - QRCoder - QR code generation
  - SharpZipLib - ZIP compression
  - Ookii.Dialogs.Wpf - File dialogs

## 📜 License

MIT License - Feel free to use, modify, and distribute.

---

⭐ If you find this useful, please give it a star!