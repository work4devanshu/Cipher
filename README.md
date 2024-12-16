# Vigenère Cipher

This repository contains an implementation of a Vigenère Cipher written in Python. The cipher allows for both encryption and decryption of messages using the same key. This project was built as a practice exercise for string manipulation in Python.

## Table of Contents
- [About the Vigenère Cipher](#about-the-vigenère-cipher)
- [Features](#features)
- [Usage](#usage)
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
