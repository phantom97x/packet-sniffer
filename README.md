# Python Packet Sniffer

A lightweight network packet sniffer built with Python and Scapy. Captures live traffic and displays source/destination IPs, protocol (TCP/UDP/other), and raw payload data in real time.

## Features
- Live packet capture using Scapy's `sniff()`
- Identifies TCP and UDP traffic, labels others as "other"
- Displays source IP, destination IP, protocol, and payload (if present)

## Requirements
- Python 3
- Scapy (`pip install scapy`)
- Root/sudo privileges (required for raw socket access)

## Usage
```bash
sudo python3 sniffer.py

EXAMPLE OUTPUT
source IP     : 151.101.209.91
destination IP: 10.0.2.15
protocol      : TCP
payload:
b'\x17\x03\x03\x00W...'
