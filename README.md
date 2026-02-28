# 🔐 Ed25519 Cryptographic Ticket Signing System

A lightweight, production-ready implementation of Ed25519 digital signatures for secure ticket issuance and verification.

This repository demonstrates how to generate keys, sign structured ticket payloads, and verify authenticity using modern elliptic-curve cryptography.

---

## 📌 Overview

This project provides a minimal and secure implementation of:

- Ed25519 key generation
- Digital signature creation
- Signature verification
- Secure payload handling
- QR-ready message encoding

The goal is to provide cryptographic authenticity without relying on blockchain or external consensus mechanisms.

---

## 🧠 Why Ed25519?

Ed25519 offers:

- 128-bit security level
- Fast verification speed
- Small key sizes (32-byte public keys)
- Fixed 64-byte signatures
- Resistance to common side-channel attacks

It is widely used in modern secure systems (SSH, TLS, cryptocurrencies, etc.).

---

## 🏗 Architecture

The cryptographic flow:

1. Generate key pair
2. Construct canonical ticket payload
3. Sign payload with private key
4. Encode payload + signature into QR
5. Verify signature using public key

Security guarantees:
- Authenticity
- Integrity
- Non-repudiation

---

## ⚙️ Installation

```bash
pip install cryptography
