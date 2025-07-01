# 🔥 Demo: Basic Firewall Rules (Linux iptables)

> “A firewall without rules is like a castle without walls.”

This demo showcases how to create basic firewall rules using `iptables` on Linux. Ideal for understanding how traffic filtering works at the packet level.

---

## 📌 Objective

- Block all incoming traffic by default  
- Allow SSH (port 22) and HTTP (port 80)  
- Drop everything else  
- Allow all outbound traffic

---

## 🛠️ Step-by-step iptables Configuration

```bash
# 🧹 Clear existing rules
sudo iptables -F

# 🚫 Set default policy to DROP
sudo iptables -P INPUT DROP
sudo iptables -P FORWARD DROP
sudo iptables -P OUTPUT ACCEPT

# 🎯 Allow loopback interface
sudo iptables -A INPUT -i lo -j ACCEPT

# ✅ Allow established connections
sudo iptables -A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT

# 🔐 Allow SSH (port 22)
sudo iptables -A INPUT -p tcp --dport 22 -j ACCEPT

# 🌐 Allow HTTP (port 80)
sudo iptables -A INPUT -p tcp --dport 80 -j ACCEPT

#🔄 Save Rules (Debian-based)

```bash
sudo apt install iptables-persistent
sudo netfilter-persistent save
```

## 🧪 Test the Rules

```bash
# Should work
curl http://localhost

# Should fail
ping your_server_ip
```
## 🧠 Notes

- Default-deny strategy is considered best practice

- Always keep console access (e.g., SSH) allowed, or you risk locking yourself out

- Test on a VM first!

## 📚 References

- iptables Documentation - https://linux.die.net/man/8/iptables

- TCM Linux 100 Course: Firewall Demo Section







