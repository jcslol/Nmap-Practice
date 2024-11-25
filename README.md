# Nmap Scans and Network Analysis Examples

This repository contains examples and findings from Nmap scans conducted on a simulated network (`172.16.0.0/24`). It provides a practical guide to discovering hosts, identifying firewalls, and analyzing services.

---

## **Contents**
1. [Ping Scans](#ping-scans)
2. [Firewall Detection](#firewall-detection)
3. [Hidden Host Identification](#hidden-host-identification)
4. [Port and Service Scans](#port-and-service-scans)

---

## **Ping Scans**
- **Objective:** Discover active hosts on the network.
- **Example Command:**
  ```bash
  sudo nmap -sn 172.16.0.0/24
<img width="538" alt="1 ping" src="https://github.com/user-attachments/assets/657a187e-641b-481f-a4d4-5bb0231c7188">
 Result: Identified 2 active hosts.

## **firewall-detection**
- **Objective:** Discover hosts is likely behind to the firewall.
- **Example Command:**
  ```bash
  sudo nmap -sn 172.16.0.0/24
<img width="522" alt="2" src="https://github.com/user-attachments/assets/8e3fdfb0-87f6-4283-956b-59cbee8cc806">
Result: Host 172.16.0.32 is likely behind a firewall.


## **hidden-host-identification**
- **Objective:** Locate hosts that are not immediately discoverable.
- **Example Command:**
  ```bash
  sudo nmap -sn 172.16.0.0/24 for hidden host ip.
  <img width="522" alt="2" src="https://github.com/user-attachments/assets/b2b25d4b-2670-4dcd-a8de-ecfaf12358c8">
   Result: Host 172.16.0.32 is likely behind a firewall.
  
  Range from 172.16.0.10 to 172.16.0.20 for find hidden host port.
  <img width="583" alt="3" src="https://github.com/user-attachments/assets/fd210e5e-b849-4776-9f52-207f39d26515">
  Result: Host hidden port is 23/tcp.
  

  ## **port-and-service-scans**
- **Objective:** Identify open ports and service running on the hidden host
- **Example Command:**
  ```bash
  sudo nmap -Pn -sV 172.16.0.32
 <img width="583" alt="3" src="https://github.com/user-attachments/assets/489e1372-562c-4dbd-8903-1b8a952f5fab">
 Result: Open port is 23/tcp and hidden service is tcpwrapped.

## References
1. Nmap Official Documentation.
2. Cybrary Lab.




