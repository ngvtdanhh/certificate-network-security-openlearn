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
Allows any host to access port 80 on 192.168.1.10

### 📄 Sample ACL Rule:
```bash
access-list 101 permit tcp any host 192.168.1.10 eq 80
✅ Allows any host to access port 80 on 192.168.1.10

## 🧠 Best Practices
- Block by default, allow by exception

- Regularly review and update rules

- Follow the principle of least privilege

## 📚 References

- Cisco ACLs: https://www.cisco.com/

- RFC 2644 – Default Deny Firewall Rule
