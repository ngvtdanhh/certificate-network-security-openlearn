# 🔐 Encryption in Network Security

> “Encryption works. Properly implemented strong crypto systems are one of the few things that you can rely on.” – Edward Snowden

This note introduces the basic types of encryption used in networking and their applications.

---

## 🔄 Why Encryption Matters

- Prevents eavesdropping
- Protects data confidentiality and integrity
- Enables secure authentication

---

## 🧮 Symmetric vs Asymmetric Encryption

| Type         | Key Used               | Examples         |
|--------------|------------------------|------------------|
| 🔁 Symmetric | Same key to encrypt/decrypt | AES, DES     |
| 🔑 Asymmetric | Public/private key pair     | RSA, ECC     |

---

## 🌐 Real-World Use Cases

| Use Case           | Protocol Used  |
|--------------------|----------------|
| Secure web browsing | HTTPS (SSL/TLS) |
| Remote shell access | SSH            |
| VPN tunneling       | IPSec, WireGuard |
| Email security      | PGP/GPG         |

---

## 🧩 Hashing and Integrity

- One-way cryptographic functions
- Example: `SHA-256`, `MD5` (⚠️ outdated)
- Used in password storage, data verification

---

## 📚 References

- Let’s Encrypt: https://letsencrypt.org
- OWASP Crypto Guide: https://cheatsheetseries.owasp.org
