# Snort IDS & ELK Stack SOC Lab

## 📌 Overview
This project is a Security Operations Center (SOC) lab that simulates real-world network attack detection using Snort IDS integrated with the ELK Stack (Elasticsearch, Logstash, Kibana).

The system monitors network traffic, detects malicious activities, and visualizes security events in real time.

---

## 🏗 Architecture

The SOC Lab consists of the following components:

- Attacker Machine (Kali Linux)
- Snort IDS for network traffic monitoring
- Honeypot (SSH / Web) to simulate vulnerable services and attract attackers
- Filebeat for log shipping
- Elasticsearch for data storage & indexing
- Kibana for visualization
- Dockerized ELK Stack deployment

---

## 🍯 Honeypot Component

The project includes a Honeypot system used to simulate vulnerable services such as SSH and Web applications.

It is used to:
- Capture attacker behavior
- Log unauthorized access attempts
- Enhance visibility of real-world attack patterns

> Note: Honeypot setup was implemented as part of the team project.

---

## ⚙️ Technologies Used

- Snort IDS
- ELK Stack (Elasticsearch, Logstash, Kibana)
- Filebeat
- Linux (Ubuntu)
- Docker
- Kali Linux

---

## 🚨 Detection Capabilities

- ICMP Ping Detection
- SSH / FTP / Telnet Detection
- DNS / SMTP / POP3 Monitoring
- SMB / RDP / MySQL / LDAP Detection
- SYN Scan & Nmap Detection
- Brute Force Attacks (SSH, FTP, Telnet, SMB)
- Web Attacks (XSS, SSRF, File Upload, Admin Access)
- Suspicious Tools Detection (nmap, sqlmap, burp, nikto)
- HTTP Flood (DDoS Simulation)
- Reverse Shell Detection

---

## 🧪 Testing Scenarios

All testing scenarios used to validate the system are documented here:

👉 `docs/testing-guide.md`

Includes:
- Network scanning tests
- Brute force attacks
- Web exploitation simulations
- Service enumeration tests

---

## 📊 ELK Dashboard

The Kibana dashboards provide real-time visualization of:
- Network attacks
- Security alerts
- Traffic patterns
- Attack frequency analysis

---

## 🐳 Docker Deployment

ELK Stack was deployed using Docker containers:

- Elasticsearch container
- Kibana container
- Logstash container
  
---

## 🎯 Project Objective

To demonstrate how Intrusion Detection Systems (IDS) combined with SIEM tools can detect, analyze, and visualize cyber attacks in a controlled SOC environment.

---

## 👨‍💻 Author

**Ahmed Ehab**  
Computer Science Student - New Cairo Academy  

🔗 LinkedIn: www.linkedin.com/in/ahmed-ehab10

---

## ⭐ Notes

- Credentials and sensitive data are removed for security reasons.
- This is a simulated SOC environment for educational purposes.
