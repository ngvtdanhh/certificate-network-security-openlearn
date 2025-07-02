 🧪 Misconfiguration: Insecure or Deprecated Services

> "Services like Telnet or FTP belong in museums, not in production."

---

## 🧯 Description

Running insecure protocols (e.g., Telnet, FTP, RSH) allows attackers to sniff traffic, inject commands, or escalate privileges.

---

## 🔍 Risky Services

| Service  | Problem                         | Alternative         |
|----------|----------------------------------|---------------------|
| Telnet   | No encryption                    | SSH                 |
| FTP      | Credentials in plaintext         | SFTP / FTPS         |
| Rlogin   | Insecure authentication          | SSH                 |

---

## ✅ Recommended Fixes

- Uninstall or disable insecure services
- Replace with encrypted alternatives
- Monitor ports and protocols in use (`ss -tuln`)

---

## 📚 Related Tools

- `chkconfig`, `systemctl`, `nmap`, `telnet`, `sshd`
