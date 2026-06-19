# Testing Guide - Snort IDS & ELK SOC Lab

## Overview
This document explains the testing scenarios used to validate the Snort IDS rules and ELK stack integration.

---

## 1. ICMP Ping Test
Command:
ping <TARGET_IP>

Expected Result:
- Snort detects ICMP traffic
- Alert generated in logs

---

## 2. SSH Test
Command:
ssh <TARGET_IP>

Expected Result:
- SSH connection attempt detected
- Alert logged by Snort

---

## 3. FTP Test
Command:
ftp <TARGET_IP>

Expected Result:
- FTP connection detected

---

## 4. HTTP Test
Command:
curl http://<TARGET_IP>

Expected Result:
- HTTP request detected and logged

---

## 5. HTTPS Test
Command:
curl https://<TARGET_IP>

Expected Result:
- HTTPS traffic detected

---

## 6. Telnet Test
Command:
telnet <TARGET_IP> 23

Expected Result:
- Telnet attempt detected

---

## 7. DNS Test
Command:
nslookup google.com <TARGET_IP>

Expected Result:
- DNS query detected

---

## 8. Nmap Scan Test
Command:
nmap -sS <TARGET_IP>

Expected Result:
- SYN scan detected by Snort

---

## 9. Brute Force SSH Test
Command:
hydra -l root -P rockyou.txt ssh://<TARGET_IP>

Expected Result:
- Multiple login attempts detected
- Brute force alert triggered

---

## 10. FTP Brute Force Test
Command:
hydra -l admin -P pass.txt ftp://<TARGET_IP>

Expected Result:
- FTP brute force detected

---

## 11. Web Attack Simulation

### XSS Test
curl http://<TARGET_IP>/"<script>"

Expected Result:
- XSS attempt detected

---

### Suspicious Download
wget http://<TARGET_IP>/file

Expected Result:
- Suspicious download detected

---

## Conclusion
All tests confirm that Snort IDS successfully detects different types of network attacks and forwards logs to the ELK stack for visualization and analysis.
