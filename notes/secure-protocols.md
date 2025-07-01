# 🔗 Secure Network Protocols

> “If you're not using encryption, you're broadcasting your data to everyone.”

This note reviews secure communication protocols used in networks and explains why insecure ones should be avoided.

---

## ✅ Why Use Secure Protocols?

- Prevent data sniffing and MITM attacks
- Provide encrypted communication channels
- Ensure authentication and integrity

---

## 🔒 Secure Protocol Examples

| Protocol | Use Case                | Security Feature        |
|----------|-------------------------|--------------------------|
| HTTPS    | Web browsing            | SSL/TLS encryption       |
| SSH      | Remote shell            | Public key authentication |
| SFTP     | Secure file transfer    | Built on SSH             |
| IPsec    | VPN tunnels             | Encrypts IP packets      |
| DNSSEC   | Domain resolution       | Validates DNS records    |

---

## ❌ Deprecated/Insecure Protocols

| Protocol | Safer Alternative |
|----------|-------------------|
| FTP      | SFTP / FTPS       |
| Telnet   | SSH               |
| HTTP     | HTTPS             |

---

## 📜 Certificates & PKI

- Use of **digital certificates** to authenticate servers
- Trusted by **Certificate Authorities (CA)**
- Part of Public Key Infrastructure (PKI)

---

## 📚 References

- Mozilla SSL Config: https://ssl-config.mozilla.org
- IETF Protocols: https://www.ietf.org
