#🚨 Attack, Detect & Secure a Cloud Infrastructure (Azure)
📌 Project Overview

This project simulates a real-world enterprise cloud environment and demonstrates how cyber-attacks are performed, detected using SIEM, and mitigated through security hardening.
Students act as Red Team (Attackers) and Blue Team (Defenders).

🏗️ Infrastructure Architecture

Cloud Platform: Microsoft Azure

Virtual Network: Single VNet

Subnets:

Internal Subnet

DMZ Subnet

Virtual Machines
VM	Role	Purpose
VM-1	Internal Server	FreeIPA (LDAP/Kerberos), File Server
VM-2	Web Server (DMZ)	Apache Web Server
VM-3	SIEM Server	Wazuh (Log Monitoring & Analysis)
🔴 Phase 1 – Red Team (Attack Simulation)
Attacks Performed

Network scanning (Nmap)

SSH brute-force attempts (Hydra)

Web enumeration (Dirb)

Directory & configuration file probing

Tools Used

Nmap

Hydra

Dirb

Linux built-in tools

✔️ Attacks generated real security logs.

🔵 Phase 2 – Blue Team (Detection & Hardening)
Log Analysis

SSH logs (auth.log)

Web logs (apache2/access.log)

System logs (syslog)

Wazuh SIEM alerts

Misconfigurations Identified

Open SSH access

Weak authentication

Unrestricted network access

Default web configurations

Security Hardening

SSH hardening (key-based login, disable root)

Firewall (UFW + Azure NSG)

Network segmentation

Server and service hardening

Enhanced logging & alerts

🔁 Re-Attack & Validation

Attacks repeated after hardening

Reduced attack surface observed

Improved SIEM alerts and detection

Clear difference in logs (before vs after)

📊 Results

Stronger security posture

Improved monitoring

Effective attack detection

Enterprise-style defense architecture

📸 Screenshots

Screenshots include:

Azure deployment (with student name visible)

SIEM dashboards

Attack logs before & after hardening

🎓 Learning Outcomes

Hands-on Red Team & Blue Team experience

SOC-level log analysis

Linux & cloud security hardening

Incident detection & response skills

👤 Author

Rahul Chandrakar
Cybersecurity Project – Azure Cloud
