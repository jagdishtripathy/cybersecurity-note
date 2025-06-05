# 🛠️ Useful Linux Security Tools 
This document contains commonly used Linux tools in cybersecurity, with explanations, use-cases, and example commands for beginners.

---

## 1. **nmap** - Network Scanner
![nmap](tools-screenshot/nmap.png)
- **Purpose:** Scan networks to find live hosts and open ports.
- **Use-case:** To understand the target's network during penetration testing.
- **Basic command:**

```bash
nmap 192.168.1.1
```
This command scans the IP address 192.168.1.1 for open ports.

-   **Advanced example:**

```bash
nmap -sV -p 1-1000 192.168.1.1
```
Here, `-sV` detects service versions and `-p 1-1000` scans ports from 1 to 1000.
