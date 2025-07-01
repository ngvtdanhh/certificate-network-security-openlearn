# 🔥 Firewalls & Access Control Lists (ACLs)

> “A firewall is like a bouncer at the door of your network.”

This note explains how firewalls and ACLs help enforce network boundaries and traffic policies.

---

## 🛡️ What is a Firewall?

A security device that filters traffic based on rules. It acts as the first line of defense.

---

## 🧱 Types of Firewalls

| Type             | Description                                 |
|------------------|---------------------------------------------|
| 📦 Packet Filter  | Filters based on IP, port, protocol         |
| 📊 Stateful       | Tracks connection states                    |
| 🧰 Application    | Filters based on application-layer data     |
| 🚀 Next-Gen FW    | Combines firewall, IDS/IPS, malware filtering |

---

## 🗂️ Access Control Lists (ACLs)

ACLs define what is allowed or denied on a system or network device.

### 📄 Sample ACL Rule:
```bash
access-list 101 permit tcp any host 192.168.1.10 eq 80
```
