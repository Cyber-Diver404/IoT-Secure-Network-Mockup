# IoT-Secure-Network-Mockup
Create a detailed network map that balances security and easability 
Project Overview:
This project defines comprehensive network architecture for integrating IoT devices into a corporate environment. It addresses the Security vs. Convenience trade-off by implementing a Zero-Trust Architecture that prevents lateral movement, secures sensitive data, and reduces the impact of compromised devices through segmentation and strict access control.

Architecture:
Zone 1: Internet (untrusted)
Zone 2: DMZ (VPN, bastion host, web servers)
Zone 3: IoT network (isolated with PVLANs)
Zone 4: Core systems (AD, databases, internal apps)

Security Features:
Zero Trust Architecture (ZTA)
VLAN & PVLAN segmentation
TLS 1.3 (data in transit)
AES-256 encryption (data at rest)
Intrusion detection and prevention systems (IDS/IPS)

Tech Stack:
Diagrams.net (network design)
PowerShell (automation)
MQTT over TLS (IoT communication)

Key Highlights:
Blocks IoT device-to-device communication (prevents lateral movement)
Automated access control & decommissioning device
Real-time threat detection with SIEM
Secure remote access via VPN + MFA

Project Demo:
The demo validates the architecture through:
Isolation Verification: Proving IoT devices cannot "ping" or scan the Corporate Database.
Threat Detection: Showing real-time IDS alerts during a simulated unauthorized access attempt.
Secure access: Implementing Group Policy Objects (GPOs).

Future Enhancements:
Implementing AI-driven anomaly detection for IoT traffic patterns.
Expanding to a Hybrid-Cloud model using AWS IoT Core or Azure IoT Hub.
Integrating Hardware Root of Trust via TPM 2.0.
