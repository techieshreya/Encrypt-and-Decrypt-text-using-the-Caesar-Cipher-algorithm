# Caesar Cipher — Encrypt & Decrypt Text

> An interactive Python implementation of the classic Caesar Cipher, letting you encrypt and decrypt messages with any shift value.

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)

## Overview

The Caesar Cipher is one of the oldest known encryption techniques: each letter in a message is shifted a fixed number of positions down the alphabet. This notebook implements both encryption and decryption with a simple interactive loop — enter a message and a shift value, and get the transformed text back.

Example from the notebook:

```
Would you like to (e)ncrypt or (d)ecrypt a message? (e/d): d
Enter your message: jgnnq aqw
Enter the shift value: 2
Decrypted message: hello you
```

## How It Works

- **`caesar_cipher_encrypt(plaintext, shift)`** — shifts each alphabetic character forward by `shift` positions using modular arithmetic (`% 26`), preserving case
- **`caesar_cipher_decrypt(ciphertext, shift)`** — reverses the shift to recover the original message
- Uppercase and lowercase letters are handled independently, so case is preserved
- Any shift value works — shifts wrap around the alphabet thanks to the modulo operation
- An interactive `main()` loop lets you encrypt/decrypt repeatedly until you choose to quit

## Tech Stack

- **Python 3** — pure standard library, no external dependencies
- **Jupyter Notebook** (developed in Google Colab)

## Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/techieshreya/Encrypt-and-Decrypt-text-using-the-Caesar-Cipher-algorithm.git
   ```

2. Open `encrypt_decrypt.ipynb` in Jupyter Notebook or [Google Colab](https://colab.research.google.com/).

3. Run the cell and follow the prompts to encrypt or decrypt your message.
