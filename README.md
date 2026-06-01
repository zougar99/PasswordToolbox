# 🔑 PasswordToolbox — A Windows desktop application with 20+ security and encoding tools — password generator, encryption/decryption, hash calculator, text encoding, and more

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/zougar99/PasswordToolbox/blob/main/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/zougar99/PasswordToolbox?style=social)](https://github.com/zougar99/PasswordToolbox)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux-blue)](https://github.com/zougar99/PasswordToolbox)

> A Windows desktop application with 20+ security and encoding tools — password generator, encryption/decryption, hash calculator, text encoding, and more.

---

## 📖 Table of Contents
- [Features](#-features)
- [How It Works](#-how-it-works)
- [Tech Stack](#-tech-stack)
- [Installation](#-installation)
- [Configuration](#-configuration)
- [Usage Guide](#-usage-guide)
- [Screenshots](#-screenshots)
- [Roadmap](#-roadmap)
- [FAQ](#-faq)
- [Troubleshooting](#-troubleshooting)
- [Contributing](#-contributing)
- [License](#-license)

---

## ✨ Features
- ✔ **Password Generator** — Configurable length, character sets, pronounceable passwords
- ✔ **Encryption/Decryption** — AES-256, ChaCha20, RSA key pair generation
- ✔ **Hash Calculator** — MD5, SHA-1, SHA-256, SHA-512, bcrypt, argon2
- ✔ **Encoding Tools** — Base64, URL encoding, Hex, Binary, Rot13
- ✔ **Password Strength Meter** — Real-time entropy and crack time estimation
- ✔ **Vault** — Encrypted local storage for passwords and notes
- ✔ **Batch Mode** — Process multiple inputs from file

---

## 🔮 How It Works

```
  Input ──► Processing Pipeline ──► Output
  ┌────────┐   ┌────────┐   ┌────────┐
  │ Data   │──►│ Engine │──►│ Result │
  │ Source │   │ Logic  │   │        │
  └────────┘   └────────┘   └────────┘
```

1. **Input** — Load data from file, API, or user input
2. **Process** — Core engine applies logic/analysis/transformation
3. **Output** — Results displayed in UI, saved to file, or sent via API

---

## 💻 Tech Stack

| Component | Technology |
|-----------|-----------|
| Language | Python 3.10+ |
| UI | CustomTkinter |
| Cryptography | cryptography + hashlib + bcrypt |
| Platform | Windows |

---

## 🚀 Installation

```bash
git clone https://github.com/zougar99/PasswordToolbox.git
cd PasswordToolbox
pip install -r requirements.txt
```

---

## 📄 Configuration

Create a `config.yaml` or `.env` file in the project root:

```yaml
# Application settings
debug: false
port: 8080
theme: dark
language: en
```

---

## 🧰 Usage Guide

1. Launch: `python main.py`
2. Select tool category (Generate / Encrypt / Hash / Encode)
3. Enter input and configure options
4. Click **Run** for instant results
5. Copy or export output

---

## 🖼 Screenshots

> *(Screenshots coming soon. PRs welcome!)*

---

## 🔄 Roadmap

- 🟢 Web dashboard
- 🟡 Mobile companion app
- ⚫ API access
- ⚫ Plugin system
- ⚫ Multi-language support

---

## ❓ FAQ

### Is the vault secure?
Yes — encrypted with AES-256-GCM with PBKDF2 key derivation.

### Can I use this offline?
Yes — all tools work completely offline.

---

## 🚧 Troubleshooting

| Problem | Solution |
|---------|----------|
| **App won't start** | Check Python version (3.10+); run `pip install -r requirements.txt` |
| **No output** | Check logs in `logs/` folder; enable debug mode in config |
| **Performance issues** | Close other applications; reduce batch size in config |
| **Dependency errors** | Create fresh venv: `python -m venv .venv && source .venv/bin/activate && pip install -r requirements.txt` |

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📐 License
Distributed under the **MIT License**. See [`LICENSE`](https://github.com/zougar99/PasswordToolbox/blob/main/LICENSE) for more information.

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/zougar99">zougar99</a>
</p>
