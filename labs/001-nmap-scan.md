# 001 — Nmap Recon: TryHackMe Basic Scan

**Date:** 2025-10-17  
**Time spent:** 1.5 hrs  
**Tools used:** nmap, bash, scan.sh (custom)

## Objective
Enumerate open ports and services on a TryHackMe lab target.

## Commands
- `~/cybersec/scripts/scan.sh <target_ip>`
- Example run: `nmap -Pn -sC -sV -p- -T4 -oN ~/cybersec/scans/nmap_10.10.10.10_2025-10-17_1200.txt 10.10.10.10`

## Findings (example)
- 22/tcp open  ssh
- 80/tcp open  http  Apache httpd 2.4.x

## Evidence
- Saved scan: `scans/nmap_10.10.10.10_2025-10-17_1200.txt` (sanitized)
- Notes: Use `title_grab.py` to check web titles and Burp to intercept HTTP requests in later labs.

## Remediation / Notes
- Typical recommendations: keep services updated, minimize exposed services, and enable fail2ban/ssh hardening for SSH.
