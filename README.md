# Task 1: Scan Your Local Network for Open Ports

## 🔍 Objective
To understand basic network reconnaissance by scanning the local network for open ports using Nmap on Windows. This helps identify services that are potentially exposed and vulnerable to attack.

## 🛠 Tools Used
- **Nmap** (installed from the official site)
- **Command Prompt (Windows)**
- *(Optional)* Wireshark for packet capture

## 🧪 Steps Performed

1. **Checked IP Range**  
   Ran `ipconfig` in Command Prompt and found the local IP:  
   Example: `192.168.1.5`  
   From this, derived the subnet range: `192.168.1.0/24`

2. **Performed a TCP SYN Scan**  
   Used the following command:  
   ```bash
   nmap -sS 192.168.1.0/24 -oN scan_results.txt
