# Encryption Playground — Caesar Cipher, ROT13, Vigenère & AES-GCM Online Cipher Lab

A free, hands-on **encryption playground** and **cryptography learning lab** that runs 100% in your browser. Encrypt and decrypt messages with the classical **Caesar cipher**, **ROT13** and **Vigenère cipher**, then graduate to real modern encryption: a working **AES-256-GCM demo** powered by the Web Crypto API with PBKDF2 password-based key derivation. Perfect for cyber security students, CTF beginners and anyone curious about how encryption actually works.

**Live Demo:** https://anaskhan0009.github.io/encryption-playground/

## Features

- **Caesar cipher tool** — encrypt/decrypt with any shift 1–25, a one-click ROT13 mode, and a "show all 25 shifts" brute-force view that demonstrates why Caesar falls instantly
- **Vigenère cipher tool** — keyword-based encrypt/decrypt with proper letter-only key handling
- **AES-256-GCM encryption demo** — real authenticated encryption via WebCrypto: PBKDF2 (150,000 iterations, random salt) derives a 256-bit key from your password; every message gets a fresh random IV; output is a portable `salt:iv:ciphertext` Base64 token
- **Tamper detection** — decrypting with a wrong password or an altered token fails loudly, showing how authenticated encryption protects integrity
- **Education section** — why classical ciphers are insecure: tiny key spaces, frequency analysis, pattern leakage, no integrity, and Kerckhoffs's principle
- **Zero dependencies, zero tracking** — one self-contained HTML file; no message or password ever leaves your device

## How to Use

1. Open the [live demo](https://anaskhan0009.github.io/encryption-playground/) (or `index.html` locally).
2. Pick a tab: Caesar, Vigenère, AES-GCM, or "Why It Matters".
3. For the classical ciphers, type a message, choose a shift/keyword, and encrypt or decrypt instantly.
4. For AES-GCM, type a message and a strong password, click **Encrypt**, and share the token. The receiver pastes the token, enters the same password, and clicks **Decrypt**.

## Why Learn Ciphers This Way?

Reading about cryptography is abstract; breaking a Caesar cipher yourself — all 25 keys in one click — makes the core lesson permanent: **security comes from key size and sound design, not from hiding the method**. This online cipher lab turns the history of cryptography (Caesar, Vigenère's 300-year reign, frequency analysis) into a bridge toward modern standards like AES-GCM and ChaCha20-Poly1305 that protect HTTPS, VPNs and encrypted messengers today.

## Ethical Use

This is an **educational, defensive tool**. Classical ciphers must never protect real secrets — they are trivially breakable, and this playground shows you why. Use the AES-GCM demo to understand modern encryption, and use real encryption knowledge to protect your own data and communications. Everything runs locally; nothing is stored, logged or uploaded.

## Tech

Single self-contained `index.html` — HTML, CSS, vanilla JavaScript, Web Crypto API (AES-GCM, PBKDF2-SHA256). No frameworks, no build step.

---

Built by **Dinal Studios** — free cyber security tools and web apps.
GitHub: https://github.com/anaskhan0009

*Keywords: encryption playground, caesar cipher online, rot13 decoder, vigenere cipher tool, aes encryption online, cryptography for beginners, cipher lab, web crypto demo, learn encryption*
