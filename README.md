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

NMAP BASICS :
Option	Explanation
-sL	List scan – list targets without scanning
Host Discovery	
-sn	Ping scan – host discovery only
Port Scanning	
-sT	TCP connect scan – complete three-way handshake
-sS	TCP SYN – only first step of the three-way handshake
-sU	UDP Scan
-F	Fast mode – scans the 100 most common ports
-p[range]	Specifies a range of port numbers – -p- scans all the ports
-Pn	Treat all hosts as online – scan hosts that appear to be down
Service Detection	
-O	OS detection
-sV	Service version detection
-A	OS detection, version detection, and other additions
Timing	
-T<0-5>	Timing template – paranoid (0), sneaky (1), polite (2), normal (3), aggressive (4), and insane (5)
--min-parallelism <numprobes> and --max-parallelism <numprobes>	Minimum and maximum number of parallel probes
--min-rate <number> and --max-rate <number>	Minimum and maximum rate (packets/second)
--host-timeout	Maximum amount of time to wait for a target host
Real-time output	
-v	Verbosity level – for example, -vv and -v4
-d	Debugging level – for example -d and -d9
Report	
-oN <filename>	Normal output
-oX <filename>	XML output
-oG <filename>	grep-able output
-oA <basename>	Output in all major formats
