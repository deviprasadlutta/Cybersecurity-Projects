# John-The-Ripper-Project
Hands-on project using John the ripper for password cracking.
## Overview
This project demonstrates using john the ripper for cracking password hashes for a zip file.
## Tools Used
-Kali linux
-John thr Ripper
-Zip2John
## Commands used
-To crack the hash :
-John prasad.txt
-Zip2John prasad.zip > prasad.txt

## Results
Cracked password: devi112233.
This project is for educational purpose only. 


# Wireshark Network Analysis Project 
## Overview
This project demonstrates the use of wireshark for analysing network traffic and identifying potential vulnerabilities.
## Tools used
-Wireshark
-Hostapd
## Objectives
-Setup a basic network using the virtual router.
-use wireshark and analyse network packets for HTTP, DNS, and TCP traffic.
-identify anomalies or suspecious activity.
## Procedure
-Set up a network of two devices and connect them using the virtual router hostapd.
-use wireshark and capture live traffic.
-Exported findings into a report.
## Disclaimer
This project is for educational purpose only.

## Nmap Scan Results
This project contains the results of an Nmap Scan 
conducted on my phone's IP address.
The goal is to showcase hoe to use Nmap for network Exploration and security auditing.


# QR Code-Based Phishing Simulation

## Objective
This project demonstrates the process of simulating a phishing attack using a QR code. The simulation includes creating a fake Instagram login page hosted on a local machine and generating a QR code that redirects to the phishing page. It is designed for educational purposes to understand phishing tactics and improve cybersecurity awareness.

---

## Disclaimer
**This project is strictly for educational purposes and was conducted in a controlled environment. Unauthorized use of phishing techniques is illegal and unethical. Always adhere to ethical hacking guidelines and cybersecurity laws.**

---

## Features
- Cloning a target website (Instagram) to create a phishing page.
- Hosting the phishing page locally on a personal machine.
- Generating QR codes for easy redirection to the phishing page.
- Capturing and logging user credentials entered on the phishing page.

---

## Tools and Technologies
- **Kali Linux**
- **Zphisher tool**
- **Qrencode** (QR Code Generator)
- **Localhost Environment**

---

## Setup and Execution

### 1. Clone the Target Website
1. Launch the Zphisher tool :
   ```bash
   bash Zphisher.sh
   ```
2. Navigate through the menu options:
   - Select the instagram option
   - select Tradition login page to steal credentials
   - select Local Host to deploy attack in your local machine
   - The url will be generated that will redirect to the fake login page

### 2. Host the Phishing Page
SET automatically sets up the phishing site on your localhost, making it accessible at `http://127.0.0.1`.

### 3. Generate a QR Code
Generate a QR code for the phishing page using the `qrencode` tool:
```bash
qrencode -o phishing_qr.png "http://127.0.0.1"
```
This will save the QR code as `phishing_qr.png`.

### 4. Simulate the Attack
1. Scan the QR code within your machine or your network (e.g., with trusted colleagues in a controlled environment).
2. Monitor and log credentials entered into the phishing page using Zphisher built-in logging system.

---

## Observations
- **Effectiveness:** The QR code successfully redirected users to the fake login page.
- **Data Capture:** User credentials entered on the phishing page were logged in SET's `harvester` log file.
- **Scope:** The attack was limited to the local machine/network due to the localhost setup.

---

## Learnings
- **Phishing via QR Codes:** QR codes are a highly effective medium for phishing attacks in trusted environments.
- **Defense Strategies:**
  - Verify URLs after scanning a QR code.
  - Avoid scanning QR codes from unknown sources.
  - Use browser security alerts and enable two-factor authentication (2FA).
- **Limitations:** Hosting the phishing page locally restricts its reach to the local network.

---

## Safety Note
**This project is intended purely for educational purposes. Unauthorized use of phishing techniques is both illegal and unethical. Always use such knowledge responsibly and for defending against cyber threats.**  
**- Deviprasad**

---

## License
This project is licensed under the [MIT License](LICENSE).
