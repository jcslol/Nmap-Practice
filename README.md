# Nmap Scans and Network Analysis Examples

This repository contains examples and findings from Nmap scans conducted on a simulated network (`172.16.0.0/24`). It provides a practical guide to discovering hosts, identifying firewalls, and analyzing services.

---

## **Contents**
1. [Ping Scans](#ping-scans)
2. [Firewall Detection](#firewall-detection)
3. [Hidden Host Identification](#hidden-host-identification)
4. [Port and Service Scans](#port-and-service-scans)
5. [Findings Summary](#findings-summary)

---

## **Ping Scans**
- **Objective:** Discover active hosts on the network.
- **Example Command:**
  ```bash
  sudo nmap -sn 172.16.0.0/24

#cybrary
