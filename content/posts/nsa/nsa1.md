+++
title = 'Vorlesung 2: Ethics and Laws, Network Access Layer'
date = 2025-04-14T18:32:03+02:00
categories = ['NSA']
tags = []
draft = false
+++

### ⚖️ Ethics and Laws – IT Security and Responsibility

**🎯 Lecture Objectives**

- Understand the **risks in a connected world**
- Learn the **goals of IT security**
- Explore **types of cyberattacks** and related **legal aspects**
- Reflect on **ethical issues** in data handling and protection

---------------------------------------

### 🛡️ Key IT Security Concepts

|**Concept**|**Description**|
|------|---|
|**IT Security**|Protection of digital systems and data against threats like hacking, malware|
|**Information Security**|Broader term – includes physical and analog data protection as well|
|**Cybersecurity**|Focused on protecting information in internet-connected environments|

---------------------------------------

### 🎯 Protection Goals (CIA Triad)

|**Goal**|**Meaning**|
|------|---|
|**Confidentiality**|Only authorized individuals can access the information|
|**Integrity**|Data must remain accurate and unaltered|
|**Availability**|Systems and data must be accessible when needed|

📌 **Example**:
If a hospital’s patient data system is hacked and made unavailable during an emergency, it violates the **availability** principle.

---------------------------------------

### 💥 Types of Cyberattacks

|**Attack Model**|**Description**|**Example**|
|------|---|---|
|**M:1**|Many attackers target a single victim|Distributed Denial of Service|
|**1:N**|One attacker targets multiple victims|Ping scan or phishing email|
|**M:N**|Multiple attackers target multiple victims|Spam, botnets|
|**1:1**|One attacker targets one specific victim|Targeted port scan|

---------------------------------------

### 👩‍💻 Ethical Aspects of Hacking

|**Type**|**Role & Intention**|
|------|---|
|**White Hat**|Ethical hackers – help organizations improve security (e.g., penetration testers)|
|**Black Hat**|Malicious hackers – exploit vulnerabilities for personal gain or harm|
|**Gray Hat**|Act without malicious intent, but without permission either|

---------------------------------------

### 📜 Legal Framework

|**Law / Regulation**|**Description**|
|------|---|
|**GDPR (General Data Protection Regulation)**|EU regulation for data protection and privacy. Ensures user rights and imposes strict fines for violations.|

📌 **Example**: A company leaking customer data without consent can be fined **up to €20 million or 4% of global revenue**.

---------------------------------------

### 🚨 Network Threats

#### 🔍 Passive vs. Active Attacks

|**Type**|**Description**|**Example**|
|------|---|---|
|**Passive**|Monitoring or eavesdropping|Traffic analysis, packet sniffing|
|**Active**|Modifying or disrupting traffic|DoS attack, man-in-the-middle|

---------------------------------------

### 🧬 MAC Address Spoofing & ARP Poisoning

#### 🔄 Positive Use of MAC Spoofing

|**Use Case**|**Description**|
|------|---|
|**Privacy Protection**|Devices (like smartphones) can randomize their MAC address to prevent tracking|

📌 **Example**: In Windows 10, MAC randomization can be enabled in Wi-Fi settings to avoid location tracking.


#### 🚨 Negative Use – ARP Poisoning 

|**Concept**|**Description**|
|------|---|
|**ARP Poisoning**|An attacker sends forged ARP packets to a target, making it believe the attacker is the gateway|
|**Man-In-The-Middle**|Attacker intercepts traffic between two devices by misdirecting network communication|

📌 **Example**: Workstation A sends data to the attacker's device, believing it's the gateway → The attacker can read, modify, or drop the traffic.

#### 🔐 Countermeasures

|**Method**|**Function**|
|------|---|
|**IEEE 802.1X Authentication**|Ensures only authenticated devices can access the network|
|**ARP Monitoring Tools**|Tools like **Snort** can detect unusual ARP activity to flag attacks|

#### 🧪 Practical Exercise – Wireshark

- Use **Wireshark** to analyze the `.pcap` file `arp-spoofing.pcap`
- Objective: Detect ARP spoofing attacks by identifying abnormal ARP communication
- Look for: Unexpected duplicate IP-MAC mappings, frequent ARP replies, or unprompted ARP broadcasts

---------------------------------------

### 🖧 Ethernet & Switch Port Authentication

|**Concept**|**Description**|
|------|---|
|**Ethernet**|The standard protocol for LANs using MAC addresses for communication|
|**Switch Port Authentication (802.1X)**|Limits network access to trusted, authenticated devices only|

📌 **Example**:
University campus Wi-Fi often uses **802.1X authentication**: students must log in using their university credentials to access the network, ensuring unauthorized devices are blocked.

