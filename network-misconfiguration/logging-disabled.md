# 📉 Misconfiguration: Logging Disabled or Ignored

> "If it’s not logged, it didn’t happen."

---

## 🧯 Description

Without proper logging, security incidents may go unnoticed. Logs are also essential for forensic investigation.

---

## ⚠️ Common Mistakes

- Logging disabled by default
- Logs not centralized or rotated
- No alerting on anomalies

---

## ✅ Recommended Fixes

- Enable logging for firewalls, SSH, web servers
- Use `rsyslog`, `journald`, or centralized logging (e.g., ELK)
- Rotate logs regularly (`logrotate`)
- Monitor `/var/log/auth.log`, `/var/log/syslog`, etc.

---

## 📚 Related Tools

- `journalctl`, `logrotate`, `syslog-ng`, `fail2ban`, `Splunk`, `Graylog`
