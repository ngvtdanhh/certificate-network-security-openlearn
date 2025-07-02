# 📡 Misconfiguration: Plaintext Data Transmission

> "Sending passwords over HTTP is like shouting them in public."

---

## 🧯 Description

Transmitting sensitive data over unencrypted channels exposes it to interception via sniffing or MITM attacks.

---

## ⚠️ Common Issues

- Login forms over HTTP
- Email or API data sent without TLS
- No SSL enforcement on web servers

---

## ✅ Recommended Fixes

- Enforce HTTPS (TLS 1.2+)
- Disable unencrypted services (e.g., POP3, IMAP)
- Use tools like `Let's Encrypt` for SSL certs

---

## 🧪 Test It Yourself

```bash
curl http://example.com/login -v
# Check if sensitive data is sent in plain text
```


## 📚 Related Tools

- curl, tcpdump, Wireshark, SSL Labs Scanner

