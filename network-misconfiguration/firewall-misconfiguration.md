# 🔥 Misconfiguration: Poor Firewall Rules

> "A misconfigured firewall is worse than no firewall at all."

---

## 🧯 Description

Incorrect firewall configurations can allow unauthorized access or block legitimate traffic, undermining both security and usability.

---

## ⚠️ Common Mistakes

- Allowing all traffic (`iptables -A INPUT -j ACCEPT`)
- Using overly broad rules (e.g., `ALLOW ALL`)
- Not filtering outgoing traffic

---

## 🔍 Example

```bash
sudo iptables -A INPUT -j ACCEPT  # 👎 Allow everything!
```

## ✅ Recommended Fixes

- Set default policy to DROP

- Allow specific traffic only (e.g., port 22, 80)

- Regularly audit firewall rules

- Backup config before changes

## 📚 Related Tools

- iptables, ufw, firewalld, nftables


