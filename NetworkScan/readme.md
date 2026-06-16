# Network Scan – Home Lab Project

## Overview
Used nmap to scan my virtual home lab network to discover active hosts, identify open ports, and running services 

## Tools Used
- nmap 7.98
- Ubuntu 26.04 (ARM) running in UTM on macOS
- Linux terminal

## What I Did
- Set up isolated Ubuntu VM
- Used `ip a` to identify VM subnet
- Ran a service version scan across the /24 subnet
- Analyzed results to identify active hosts, open ports, and running services

## Findings
- 2 active hosts detected
- Host 1 (192.168.64.1): UTM gateway — ports 53 (DNS), 5000 and 7000, 49152 
- Host 2 (192.168.64.2): Local VM — all 1000 ports closed

## What This shows
- Network reconnaissance using nmap
- Understanding of subnetting (/24)
- Ability to interpret port scan results

## What command I ran 
1. Install the latest version of Nmap: `sudo apt install nmap -y` 
2. Find your network range: `ip a`
3. Run the scan: `nmap -sV <your-network-range>/24



