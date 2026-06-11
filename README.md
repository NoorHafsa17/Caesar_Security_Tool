# Caesar Security Tool 🔐

**Author:** Noor Hafsa  
**Project:** — Caesar Cipher (Educational + Defensive Demo)

---

## Project summary
This repository contains a Python implementation of the **Caesar Cipher** with added educational security features to demonstrate both attack vectors and defensive controls. The tool is intended for learning and awareness — not for real-world secret management.

**Features**
- Encrypt / Decrypt (Caesar cipher)
- Brute-force demo (shows all 25 possible shifts)
- File-based encrypt/decrypt support
- Simple suspicious-content detector (URL & phishing-like keyword patterns)
- Basic rate-limiter for brute-force attempts (educational)
- Local logging of metadata (no plaintext or keys should be logged)
- Optional secure demo using `cryptography.fernet` (requires package)

---

## Files in this repo
- `caesar_cipher.py` — main script (CLI)
- `README.md` — this file
- (optional) `requirements.txt` — list of dependencies (see below)

---

## Requirements
- Python 3.8+ recommended
- Optional (for the Fernet demo): `cryptography`

Install dependencies (optional):
```bash
pip install -r requirements.txt

How to run (CLI)

Open terminal / PowerShell and change to this project folder:

cd path/to/PRODIGY_CS_01


Run the script:

python caesar_cipher.py


Follow the on-screen menu:

1) Encrypt text (console)
2) Decrypt text (console)
3) Brute-force a ciphertext (console)
4) Scan text for suspicious content (phishing detector)
5) File: encrypt -> write file
6) File: decrypt -> write file
7) Secure demo (Fernet) [optional]
8) Exit

Example usage (quick)

Encrypt text:

Choice 1 → message: hello → shift: 3 → output khoor

Brute-force:

Choice 3 → ciphertext: khoor → you will see Shift 03: hello among results

File encrypt:

Choice 5 → input: sample_text.txt → output: encrypted.txt → shift: 4
