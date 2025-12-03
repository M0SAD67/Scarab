# Scarab🔐

A comprehensive Flutter application for learning and performing various cryptographic operations. This app provides an interactive way to understand classical and modern encryption algorithms with detailed visualizations and step-by-step solutions.

## ✨ Features

### 🔑 Supported Algorithms
The app supports a wide range of cryptographic methods, categorized for easy navigation:

*   **Classical Ciphers**:
    *   **Caesar Cipher**: Simple substitution with shift visualization.
    *   **Vigenère Cipher**: Polyalphabetic substitution with table visualization.
    *   **Rail Fence Cipher**: Transposition with ZigZag pattern visualization.
    *   **Playfair Cipher**: Digraph substitution using a 5x5 matrix.
    *   **Hill Cipher**: Polygraphic substitution using matrix multiplication.
    *   **Columnar Transposition**: Grid-based rearrangement.
    *   **Row Transposition**: Row-based rearrangement.
    *   **Affine Cipher**: Mathematical substitution ($ax + b$).

*   **Modern Ciphers**:
    *   **RSA**: Asymmetric encryption with key generation and modular exponentiation steps.
    *   **AES**: (Planned/In Progress) Symmetric block cipher.

### 🛠️ Key Features

*   **Interactive Visualizations**:
    *   **"Solution Method"**: A dedicated feature to view the step-by-step process of encryption/decryption.
    *   **Playfair Matrix**: Visualizes digraph movements with distinct colored arrows, wrap-around curves, and cell highlighting.
    *   **Rail Fence ZigZag**: Draws the actual zigzag path of characters.
    *   **Matrix Operations**: Shows matrix multiplication for Hill cipher.

*   **Advanced Key Generation**:
    *   **Context-Aware**: Generates keys suitable for the selected algorithm (e.g., 5x5 matrix for Playfair, coprime pairs for Affine).
    *   **Secure Randomness**: Uses cryptographically secure random number generators.
    *   **RSA Key Gen**: Generates Public/Private key pairs with adjustable prime size (Educational vs. Secure modes).

*   **History & Management**:
    *   **Encryption History**: Automatically saves your operations.
    *   **Smart Duplication**: Repeated operations increment a counter instead of cluttering the list.
    *   **Details View**: View full input/output, keys, and timestamp.

*   **Educational Tools**:
    *   **Strict Validation**: Real-time feedback on key validity (e.g., coprime checks, matrix invertibility).
    *   **Educational Mode**: Limits RSA primes to small numbers (<= 100) for easier understanding of the math.

*   **Localization**:
    *   Full support for **English** and **Arabic** (RTL layout supported).

## 🚀 Future Enhancements

*   [ ] **AES Visualization**: Detailed step-by-step view of AES rounds (SubBytes, ShiftRows, MixColumns).
*   [ ] **File Encryption**: Support for encrypting images, videos, and documents.
*   [ ] **Hash Functions**: Visualization for MD5, SHA-256 hashing processes.
*   [ ] **Steganography**: Hiding text within images.
*   [ ] **Network Analysis**: Simulating Man-in-the-Middle attacks for educational purposes.

## 📱 Screenshots

*(Add your screenshots here)*

## 📦 Installation

1.  Clone the repository:
    ```bash
    git clone https://github.com/yourusername/cryptography-app.git
    ```
2.  Navigate to the project directory:
    ```bash
    cd cryptography-app
    ```
3.  Install dependencies:
    ```bash
    flutter pub get
    ```
4.  Run the app:
    ```bash
    flutter run
    ```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
