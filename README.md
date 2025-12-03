# 🔐 Scarab

<div align="center">
<!-- <img src="assets/icons/app_icon.png" alt="M O S A Logo" width="150" height="150"/> -->
  
![Scarab](https://img.shields.io/badge/Scarab-00D4AA?style=for-the-badge&logo=flutter&logoColor=white)

**Comprehensive Cryptography Learning & Tooling App with Interactive Visualizations**

[![Flutter](https://img.shields.io/badge/Flutter-3.0+-02569B?style=flat&logo=flutter)](https://flutter.dev)
[![Dart](https://img.shields.io/badge/Dart-3.0+-0175C2?style=flat&logo=dart)](https://dart.dev)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Android-3DDC84?style=flat&logo=android)](https://www.android.com)

[Features](#-features) • [Installation](#️-installation) • [Usage](#-usage) • [Screenshots](#-screenshots) • [Developer](#-developer)

</div>

---

## 📦 Download

<div align="center">

### 📲 **Get the Latest Release**

You can download the latest version of **Scarab** below 👇

[![Download APK](https://img.shields.io/badge/⬇️_Download-APK-blue?style=for-the-badge&logo=android)](https://github.com/M0SAD67/Scarab/releases/download/V1.0.0/Scarab.apk)


Or visit the **[Releases](https://github.com/M0SAD67/Scarab/releases/)** page to see all available versions.
</div>

---

### 🛠️ How to Install (Android)

1. Download the `.apk` file from the link above.  
2. Open the file on your Android device.  
3. Allow installation from unknown sources (if prompted).  
4. Launch **Scarab** and start encrypting!

---

## 🎯 Overview

**Scarab** is a powerful educational and utility app built with Flutter, designed to demystify cryptographic algorithms. It offers detailed step-by-step visualizations, secure key generation, and a modern, user-friendly interface.

### ✨ Key Features

#### 🔑 **Supported Algorithms**
- **Classical Ciphers**:
  - **Caesar Cipher**: Simple shift substitution.
  - **Vigenère Cipher**: Polyalphabetic substitution.
  - **Rail Fence Cipher**: ZigZag transposition.
  - **Playfair Cipher**: 5x5 Matrix digraph substitution.
  - **Hill Cipher**: Matrix multiplication polygraphic cipher.
  - **Affine Cipher**: Mathematical substitution ($ax + b$).
  - **Transposition**: Columnar and Row-based rearrangement.
- **Modern Ciphers**:
  - **RSA**: Asymmetric encryption with key generation.

#### 🎨 **Interactive Visualizations**
- **"Solution Method"**: Step-by-step breakdown of every operation.
- **Playfair Matrix**:
  - **All Arrows View**: See all transformations at once.
  - **Interactive Player**: Step through each digraph.
  - **Wrap-Around Curves**: Visual indication of row/column wrapping.
- **Rail Fence ZigZag**: Visual path of characters.
- **Hill Matrix**: Visual matrix multiplication steps.

#### 🛡️ **Security & Tools**
- **Advanced Key Generation**:
  - **Context-Aware**: Generates valid keys for specific algorithms (e.g., Coprime pairs for Affine).
  - **Secure Randomness**: Uses cryptographically secure RNG.
  - **RSA Key Gen**: Adjustable prime sizes (Educational vs. Secure).
- **Strict Validation**: Real-time feedback on key validity.
- **Educational Mode**: Limits RSA primes to small numbers for learning.

#### 📝 **History & Management**
- **Smart History**: Automatically saves operations.
- **Duplication Handling**: Increments counter for repeated operations.
- **Detailed View**: Inspect full input, output, keys, and timestamps.
- **Clipboard Integration**: One-tap copy for text and keys.

#### 🌐 **Languages**
- Arabic support (RTL)
- English support

---

## 🛠️ Tech Stack

### Frontend
- **Flutter 3.0+** - Main framework
- **Dart 3.0+** - Programming language

### Core Libraries

#### Cryptography & Math
```yaml
crypto: ^3.0.3                 # Hashing algorithms
# Custom implementations for Classical & RSA
```

#### Data & Storage
```yaml
shared_preferences: ^2.0.15    # History storage
file_picker: ^10.3.7           # File selection
path_provider: ^2.1.5          # File system access
```

#### User Interface
```yaml
dynamic_color: ^1.8.1          # Material 3 dynamic theming
intl: any                      # Localization
flutter_localizations: sdk     # Flutter l10n support
```

---

## 📋 Requirements

### System
- **Android**: 5.0 (API 21) or higher
- **iOS**: 11.0 or higher

### Development Tools
- Flutter SDK 3.0 or higher
- Dart SDK 3.0 or higher
- Android Studio / VS Code

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/M0SAD67/cryptography-app.git
cd cryptography-app
```

### 2️⃣ Install Dependencies

```bash
flutter pub get
```

### 3️⃣ Run the App

```bash
# For development
flutter run

# Build APK
flutter build apk --release
```

---

## 📱 Usage

### Encryption/Decryption
1. Select an algorithm from the home screen.
2. Enter your text.
3. Enter or generate a key.
4. Tap **Encrypt** or **Decrypt**.

### Viewing Solutions
1. After an operation, tap the **History** icon.
2. Tap on the history item.
3. Click **"Solution Method"** (or "طريقة الحل").
4. Explore the step-by-step visualization.

### Key Generation
1. Tap the **Key** icon in the input field.
2. Configure settings (Length, Educational Mode, etc.).
3. Tap **Generate**.

---

## 📂 Project Structure

```
cryptography-app/
├── lib/
│   ├── main.dart                      # Entry point
│   ├── screens/
│   │   ├── home_screen.dart           # Algorithm selection
│   │   ├── encryption_screen.dart     # Main operation screen
│   │   ├── history_screen.dart        # History list
│   │   └── key_generation_screen.dart # Key generator
│   ├── services/
│   │   ├── encryption_service.dart    # Core logic facade
│   │   ├── history_service.dart       # Storage logic
│   │   └── ciphers/                   # Algorithm implementations
│   ├── widgets/
│   │   └── solution_method_widget.dart# Visualization engine
│   └── models/
│       └── encryption_model.dart      # Data models
├── assets/
│   └── icons/                         # App icons
├── pubspec.yaml                       # Dependencies
└── README.md                          # This file
```

---

## 🎨 Screenshots

### Home Screen
- Categorized algorithms
- Modern Material 3 Design
- Dark/Light mode support

### Visualization
- Interactive Playfair matrix
- Detailed Vigenère table
- Step-by-step RSA math

### History
- Organized list with badges
- Detailed inspection sheet

---

## 🤝 Contributing

Contributions are welcome! If you'd like to contribute:

1. Fork the project
2. Create a new branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Future Development Ideas
- [ ] AES Visualization
- [ ] File Encryption Support
- [ ] Hash Function Visualizations
- [ ] Steganography Tools

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2025 Mohamed (MOSAD)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
```


## 👨‍💻 Developer

**Mohamed (MOSAD)**

- GitHub: [@M0SAD67](https://github.com/M0SAD67)
- Email: mhmdaldhshwry280@gmail.com

### 🙏 Special Thanks
- **Flutter Team** - Amazing framework
- **Dart Team** - Powerful language

---

## 🐛 Known Issues

1. **Large Primes**: RSA generation with very large primes may be slow on older devices.

---

## 📞 Support & Contact

If you encounter an issue or have a suggestion:

- Open an [Issue](https://github.com/M0SAD67/cryptography-app/issues) on GitHub
- Email me at [mhmdaldhshwry280@gmail.com](mailto:mhmdaldhshwry280@gmail.com)

---

## 🌟 Support the Project

If you like the project:
- ⭐ Star the project on GitHub
- 🔀 Share the project with friends
- 🐛 Report bugs
- 💡 Suggest new features

---

<div align="center">

**Made with ❤️ in Egypt**

[![GitHub](https://img.shields.io/badge/GitHub-M0SAD67-181717?style=for-the-badge&logo=github)](https://github.com/M0SAD67)

</div>
