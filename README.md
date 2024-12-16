# Vigenère Cipher

This repository contains an implementation of a Vigenère Cipher written in Python. The cipher allows for both encryption and decryption of messages using the same key. This project was built as a practice exercise for string manipulation in Python.

## Table of Contents
- [About the Vigenère Cipher](#about-the-vigenère-cipher)
- [Features](#features)
- [Usage](#usage)
- [How it Works](#how-it-works)
- [Installation](#installation)
- [Examples](#examples)
- [License](#license)

---

## About the Vigenère Cipher
The Vigenère Cipher is a method of encrypting alphabetic text by using a simple form of polyalphabetic substitution. It uses a keyword where each letter of the keyword defines a shift for the corresponding letter in the message. Unlike simple Caesar Ciphers, the Vigenère Cipher employs multiple Caesar shifts based on the letters of a key.

## Features
- **Encrypt Messages:** Encrypt plaintext messages using a provided key.
- **Decrypt Messages:** Decrypt ciphertext messages using the same key.
- **Character Preservation:** Non-alphabetic characters (like spaces, numbers, and punctuation) are preserved as-is.
- **Case Insensitivity:** Input messages are automatically converted to lowercase to simplify encryption.

## Usage
The cipher can be used to encrypt or decrypt text messages. By default, it encrypts the message. To decrypt, simply set the `direction` parameter to `-1`.

## How it Works
1. **Lowercase Conversion:** All letters in the message are converted to lowercase.
2. **Non-letter Handling:** Characters that are not letters (like punctuation and numbers) are left unchanged.
3. **Key Repetition:** The key is repeated to match the length of the message.
4. **Offset Calculation:** Each letter of the message is shifted by an amount corresponding to the position of the key's letter.
5. **Encryption/Decryption:** Characters are shifted forward for encryption (`direction=1`) and backward for decryption (`direction=-1`).

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/cipher.git
   ```
2. Navigate to the project directory:
   ```bash
   cd cipher
   ```
3. Run the cipher notebook.

## Examples
### Encrypt Example
**Input:**
```
Message: "keep going strong"
Key: "success"
```
**Output:**
```
Encrypted Message: "cygr kgafa uvvgfy"
```

### Decrypt Example
**Input:**
```
Encrypted Message: "cygr kgafa uvvgfy"
Key: "success"
```
**Output:**
```
Decrypted Message: "keep going strong"
```
