# 🧪 Demo: Packet Sniffing Simulation with tcpdump

> “To defend a network, you must first understand what flows through it.”

This demo uses `tcpdump` to capture and analyze network traffic. It's a lightweight yet powerful tool to simulate packet analysis in a Linux terminal.

---

## 📌 Objective

- Capture basic traffic
- Filter traffic by port and protocol
- Analyze suspicious traffic patterns

---

## 🛠️ Installation

```bash
sudo apt update
sudo apt install tcpdump
```

## 🔍 Basic Usage

```bash
# Capture packets on eth0 interface
sudo tcpdump -i eth0

# Capture only TCP traffic on port 80
sudo tcpdump -i eth0 tcp port 80

# Save packets to a file
sudo tcpdump -i eth0 -w capture.pcap

# Read saved capture
tcpdump -r capture.pcap
```

## 📄 Example Output

```bash
14:33:48.123456 IP 192.168.1.5.54321 > 192.168.1.10.http: Flags [S], seq 0, win 65535
```

## 🧠 Real-World Use Cases

- Identify unusual outbound connections

- Analyze unencrypted traffic (e.g., plain HTTP)

- Detect scanning behavior or brute-force attempts

## ⚠️ Ethical Reminder

Use packet sniffing only on systems you own or have explicit permission to test.

## 📚 References

- tcpdump man page - https://man7.org/linux/man-pages/man8/tcpdump.8.html

- Wireshark (GUI alternative): https://www.wireshark.org/
