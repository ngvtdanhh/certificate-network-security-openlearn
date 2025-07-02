# 🔑 Misconfiguration: Weak or Default Credentials

> "Most breaches don't require brute force — they just require no change."

---

## 🧯 Description

Default usernames and passwords (e.g., `admin:admin`) are often indexed in public databases. Attackers routinely scan and test them.

---

## 🔍 Example

- MySQL: `root:` (no password)
- Router: `admin:admin`
- SSH: `root:toor`

---

## 🛡️ Attack Techniques

- Credential stuffing
- Brute force attacks
- Automated scanners (e.g., Hydra, Medusa)

---

## ✅ Recommended Fixes

- Disable default accounts or change passwords immediately
- Enforce strong password policies
- Use SSH key authentication
- Monitor failed login attempts (`/var/log/auth.log`)

---

## 📚 Related Tools

- `Hydra`, `Fail2Ban`, `pam_pwquality`
