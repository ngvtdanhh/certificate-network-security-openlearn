# 🔓 Misconfiguration: Open and Unfiltered Ports

> "Every open port is a potential entry point."

---

## 🧯 Description

Leaving unnecessary ports open — especially to the public internet — expands the attack surface and increases risk of scanning, enumeration, and exploitation.

---

## 🚫 Common Mistakes

- Running services on default ports without firewall
- Exposing development tools (e.g., phpMyAdmin, Redis)
- Forgetting to close test services

---

## 🔍 Example

```bash
nmap -p- 192.168.1.100
# Open ports found: 21 (FTP), 23 (Telnet), 3306 (MySQL)
```
