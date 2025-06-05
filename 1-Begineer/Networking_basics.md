# 🌐 Basic Networking Concepts
If you're starting your cybersecurity journey, you must understand how devices communicate over a network. This guide covers foundational networking concepts explained in simple terms, with commands and examples to practice.

---

## 📘 What is Networking?

Networking is the process of connecting two or more devices so that they can share information. In cybersecurity, understanding how data flows in a network helps in analyzing traffic, identifying threats, and exploiting or securing systems.

---

## 🧩 Key Concepts and Definitions

| Term           | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| **IP Address** | Logical address used to identify a device on a network (e.g., 192.168.1.10) |
| **MAC Address**| Physical address burned into your device’s network interface (e.g., 00:1A:...) |
| **DNS**        | Converts domain names (like `google.com`) into IP addresses                 |
| **DHCP**       | Automatically assigns IP addresses to devices in a network                  |
| **Gateway**    | Acts as an access point to another network, usually the router              |
| **Subnet**     | Smaller division of a network, defined using a subnet mask (e.g., 255.255.255.0) |
| **Port**       | A logical channel to identify specific processes/services (e.g., port 80 for HTTP) |

---

## 🔢 IP Address (Internet Protocol Address)

An IP address is a unique identifier assigned to each device in a network.

- **IPv4 Example**: `192.168.1.1`
- **IPv6 Example**: `2001:0db8:85a3:0000:0000:8a2e:0370:7334`

There are two main types:
- **Public IP**: Visible on the internet
- **Private IP**: Used in LANs (Local Area Networks)

### 🧪 Practice:
```bash
ip a        # Shows IP address in Linux
ipconfig    # Use in Windows
🔐 MAC Address (Media Access Control)
```
A MAC address is a **hardware address** that identifies your device's NIC (Network Interface Card). It's static and unique for every device.

### 🧪 Practice:
```bash
ip link show        # Linux
getmac              # Windows
```
* * * * *

🌐 DNS (Domain Name System)
---------------------------

DNS translates human-friendly domain names into IP addresses that computers understand.

### Example:

`google.com` → `142.250.182.14`

Without DNS, you'd have to remember the IP of every website.

### 🧪 Practice:
```bash
nslookup github.com
dig github.com
```
* * * * *

📤 DHCP (Dynamic Host Configuration Protocol)
---------------------------------------------

DHCP automatically assigns:

-   IP address

-   Subnet mask

-   Default gateway

-   DNS server

This avoids the need to manually configure network settings.

* * * * *

🧪 Common Networking Commands
-----------------------------

| Command | Purpose |
| --- | --- |
| `ping <host>` | Checks if a host is reachable and shows response time |
| `traceroute <host>` | Shows the route packets take to reach the destination |
| `nslookup <domain>` | Resolves a domain name to its IP address |
| `whois <domain>` | Displays domain ownership and registration info |
| `netstat -tuln` | Lists listening ports and active connections |
| `ifconfig` / `ip a` | Displays current IP configuration |

* * * * *

🧭 Public vs Private IP
-----------------------

| Type | Example Range | Use Case |
| --- | --- | --- |
| **Public** | Assigned by ISP | Access internet |
| **Private** | `192.168.x.x`, `10.x.x.x` | Used in internal networks (LAN) |

* * * * *

🔌 Ports and Protocols
----------------------

Each service runs on a specific **port number** and uses a **protocol** (TCP or UDP). For example:

| Service | Port | Protocol |
| --- | --- | --- |
| HTTP | 80 | TCP |
| HTTPS | 443 | TCP |
| DNS | 53 | UDP/TCP |
| SSH | 22 | TCP |
| FTP | 21 | TCP |

* * * * *

🎯 Real-Life Scenario: Website Access
-------------------------------------

1.  You type `example.com` in browser.

2.  DNS converts domain to IP.

3.  Your device sends an HTTP request via port 80.

4.  Server responds and loads the page.

* * * * *

🧠 Key Takeaways
----------------

-   IP & MAC addresses uniquely identify devices.

-   DNS helps resolve human-readable names.

-   DHCP simplifies network setup.

-   Basic tools like `ping`, `traceroute`, and `nslookup` are essential in pentesting.

-   Understanding ports and services is critical for scanning and exploitation.
