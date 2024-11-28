# Kali-LAN Project

## Overview
The **Kali-LAN Project** is a hands-on learning initiative designed to provide a real-world environment for analyzing and experimenting with low-level attacks, "living off the land" (LOTL) techniques, and advanced network operations. The lab combines elements of cybersecurity and network engineering, offering a unique opportunity to explore real-world scenarios in a controlled, physical environment.

### Project Objectives:
1. **Build a physical lab** with various legacy and modern devices.
2. **Simulate a corporate-style network** to explore vulnerabilities, attacks, and defenses.
3. **Reinforce concepts** from cybersecurity and network engineering programs.
4. **Provide help desk training** opportunities for LAN device management and troubleshooting.

---

## Goals

### Cybersecurity Education:
- Understand and analyze low-level attacks (e.g., reverse shells, credential theft, persistence techniques).
- Practice network reconnaissance, privilege escalation, and lateral movement.
- Explore endpoint vulnerabilities and LOTL techniques.
- Develop effective defenses and incident response strategies.

### Network Engineering Skills:
- Configure and manage network devices (e.g., Cisco Catalyst switches, wireless access points).
- Implement VLANs, routing, and subnetting for network segmentation.
- Analyze network traffic for security and performance insights.

### Help Desk Concepts:
- Train on device setup, maintenance, and troubleshooting.
- Simulate real-world issues like misconfigurations and device failures.
- Develop communication skills for explaining technical problems and solutions.

---

## Lab Setup

### Network Topology:
The lab is based on a physical network with segmented VLANs for isolated testing.

**Devices**:
- **Windows 7 laptop** (legacy machine).
- **D-Link DIR-601 wireless access point** (IoT and wireless mesh simulations).
- **Cisco Catalyst 3560 switch** (core switch with VLAN capabilities).
- **Kali Linux attacker machine** (penetration testing and analysis).
- **Virtualized servers** on a Type-2 hypervisor (Active Directory, email, and file servers).
- **Miscellaneous devices** (printers, IoT devices, routers, hypervisors and user workstations).

---

### Key Components:

#### VLANs:
- Segregate the network into functional zones:
  - **IoT VLAN** for D-Link DIR-601 and IoT devices.
  - **Corporate VLAN** for workstations and servers.
  - **Attack VLAN** for Kali Linux and testing environments.

#### Legacy Device Integration:
- Focus on vulnerabilities in older systems like Windows 7 and legacy firmware (e.g., D-Link DIR-601).
- Demonstrate low-level attacks, persistence, and defense mechanisms.

#### Active Directory Structure:
- Simulate a corporate environment with an **orkid.local domain**, including users and groups:
  - **Organizational Units (OUs)**: VANDA, CATTLEYA, and CATASETUM.
  - Simulated employees: `mpalmer`, `swilson`, etc.
- Provide realistic scenarios for lateral movement and privilege escalation.

#### Wireless Access Point (D-Link DIR-601):
- Explore vulnerabilities such as **credential disclosure** (e.g., CVE-2018-12710).
- Simulate IoT mesh attacks and network misconfigurations.

#### Cisco Catalyst 3560:
- Test DoS attacks (e.g., CVE-2005-4258 Land Attack).
- Practice VLAN hopping and ARP spoofing.

---

## Learning Scenarios

### Cybersecurity Scenarios:
1. **Persistence and Privilege Escalation**:
   - Use reverse shells and persistence mechanisms to maintain access.
   - Demonstrate lateral movement across VLANs and the corporate domain.
   
2. **IoT Exploitation**:
   - Exploit D-Link DIR-601 vulnerabilities to gain network access.
   - Use the IoT mesh network as a foothold for larger attacks.

3. **Denial of Service (DoS)**:
   - Simulate DoS attacks on the Cisco Catalyst 3560 switch.
   - Highlight the importance of network hardening and traffic monitoring.

4. **Network Reconnaissance**:
   - Use tools like **Nmap** and **Wireshark** for active and passive mapping.
   - Identify weaknesses in configurations and access points.

---

### Network Engineering Scenarios:
1. **VLAN Management**:
   - Configure and test VLANs to isolate and secure network segments.
   - Simulate inter-VLAN routing and troubleshooting.

2. **Device Configuration and Maintenance**:
   - Manage and troubleshoot network devices (e.g., Cisco Catalyst, D-Link AP).
   - Implement access control lists (ACLs) and port security.

3. **Traffic Analysis**:
   - Use packet capture tools (e.g., **Wireshark**) to monitor performance and identify anomalies.

---

### Help Desk Training:
- Simulate common issues (e.g., forgotten passwords, misconfigured devices).
- Develop troubleshooting workflows and documentation practices.

---

## Tools and Resources

### Hardware:
- **Windows 7 laptop**.
- **D-Link DIR-601 wireless access point**.
- **Cisco Catalyst 3560 switch**.
- **Personal workstation for management**.
- *Other intermediary devices and hypervisors*

### Software:
- **Kali Linux** (penetration testing and analysis tools).
- **Virtualized servers** (Active Directory, DNS, email, file sharing).
- **Wireshark** (network traffic analysis).
- **Burp Suite** (web application testing).

### Documentation:
- Regularly document attack scenarios, defenses, and network configurations.
- Create incident response guides based on simulated attacks.

---

## Future Plans

1. **Expand Attack Scenarios**:
   - Include complex attacks like Kerberoasting, NTLM relay, and DNS spoofing.

2. **Develop Capture the Flag (CTF) Challenges**:
   - Create realistic challenges for use by cybersecurity club members.

3. **Enhance Network Hardening**:
   - Simulate red team vs. blue team exercises.

---

## Getting Started

1. Set up the hardware components and ensure all devices are connected to the lab network.
2. Configure VLANs on the Cisco Catalyst 3560 switch.
3. Install and configure the necessary software (e.g., Kali Linux, virtual servers).
4. Begin testing scenarios and document your findings.

---

## Contributors
- **Project Lead**: Dubz Hacker  
- **Help Desk Assistant**: College Roomate/Son  
- **Cybersecurity Club Members**: [Optional future collaborators]

---

## Acknowledgments
This project was inspired by the desire to create a comprehensive learning environment for both cybersecurity and network engineering students. Special thanks to the creators of tools like **Kali Linux** and **Wireshark**, and to educators who emphasize hands-on learning.

---

## Disclaimer
This project is for **educational purposes only**. Ensure all testing and attacks are conducted in a controlled lab environment and adhere to ethical guidelines. Do not use these techniques on unauthorized systems.
