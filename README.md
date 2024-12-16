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


## License
BSD 3-Clause License

Copyright (c) 2024, freeCodeCamp. All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.

Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
