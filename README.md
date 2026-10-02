# my-cyber-cheat-sheets
Hands-on technical notes and commands from my cybersecurity training.
# Cybersecurity Notes & Commands

This repository tracks my hands-on cybersecurity learning journey and technical command cheat sheets.

## 🌐 Networking Diagnostics
Useful commands for mapping networks and checking connectivity.

### Ping (Check if host is alive)
```bash
ping <TARGET_IP>
```

### Traceroute (Track packet route)
```bash
traceroute <TARGET_IP>
```

## 📡 Nmap (Network Scanning)
Basic network scanning commands learned in TryHackMe.

### Service & Script Scan
```bash
nmap -sV -sC <TARGET_IP>
```

## 📂 Web Enumeration
Tools for finding hidden directories.

### Gobuster
```bash
gobuster dir -u http://<TARGET_IP> -w /usr/share/wordlists/dirb/common.txt
