# Multi-Table + Multi-Offset Extended Caesar Cipher

[**🌐 Live Demo (More Secure!)**](https://www.kisara.art/?id=14)

[中文版](./README.md) | **English**

An enhanced implementation of the Caesar Cipher. By introducing **Dynamic Offset Sequences** and **Polyalphabetic Substitution**, it overcomes the vulnerability of traditional Caesar ciphers to frequency analysis.

---

## 📖 Introduction

Traditional Caesar ciphers use a single fixed shift for the entire text. This tool assigns a unique, randomized "Offset Sequence" to each word. This means the same letter may result in entirely different characters depending on its position and the chosen sequence.

While maintaining the lightweight and simple nature of the original cipher, this method significantly boosts resistance against basic statistical analysis—perfect for SNS message encryption or decryption games.

---

## ⚙️ How It Works

The encryption process follows this logic:

1.  **Select Offset Sequence**: A predefined offset sequence is randomly selected for each word (e.g., `"aba": [11, 3, 8, 18, 9]`).
2.  **Apply Cyclic Shift**:
    * The 1st letter of the word shifts based on the 1st value in the sequence.
    * If the word is longer than the sequence, the sequence loops.
3.  **Generate Ciphertext**: A specific sequence code (e.g., `aba`) is appended to each encrypted word, allowing the decrypter to identify the correct rule.
4.  **Non-Alphabetic Characters**: Numbers, spaces, and special symbols remain unchanged.

---

## ✨ Features

* **Dynamic Encryption**: Every encryption of the same text produces a different ciphertext.
* **Polyalphabetic Substitution**: Multiple shift steps break the fixed frequency patterns found in classic ciphers.
* **Accurate Decryption**: Built-in sequence identifiers ensure the decryption is always 100% accurate.
* **Customizable Security**: Users can define their own **屏蔽词 (Shield Words)** mapping tables and shift steps.

---

## 🚀 Usage & Security Tips

> [!TIP]
> **Security Notice**
> The public scripts for this project are not obfuscated for educational purposes. For private or sensitive use, it is recommended to:
> 1.  **Update "Shield Words"**: Redefine the **屏蔽词 (Shield Words)** mapping table in the source code.
> 2.  **Customize Steps**: Change the numerical values in the offset sequences.
> 3.  **Code Obfuscation**: Use an obfuscator on the core JavaScript to prevent others from reverse-engineering your rules.

---

## 📸 Demo

* **Encryption / Decryption**:
    ![Encryption Demo](https://www.kisara.art/zb_users/upload/2025/11/202511031762137160271995.png)
* **Dynamic Variation** (Same input, different results):
    ![Dynamic Variation Demo](https://www.kisara.art/zb_users/upload/2025/11/202511031762137190752069.png)

---

## 🛠️ Tech Stack

* **HTML5 / CSS3**: Responsive UI design.
* **JavaScript (ES6)**: Core dynamic encryption algorithm.
