title = "Maryville's Operationally Vulnerable Entity" <br>
date = "2023-05-16" <br>
description = "This project is meant to be a full service lab and mock client for use in Maryville's ISYS 490 practical cybersecurity course. Portions of this entity are from [kcycyber.org](https://kc7cyber.org). Documentation for setup will be broken down by the services that the students will provide to the fake client (MOLK dairy company)" <br>
tags = ["move","vulnerability scanning","penetration testing","open-source intelligence","log analysis","kc7"] <br>

---

## Vulnerability Scanning

**Description**: Use the Nessus server to run scans against an intentionally vulnerable server.

**Assignment**: MOLK has requested an external vulnerability scan. Log into the Nessus server to create and launch a scan against their infrastructure. Then, export the Nessus report and create your own report with the template provided. 

**Deliverable**: Vulnerability reports sent to "client" (the one in Teams & Nessus Export).

### Outline 
- VLAN this whole thing
- ProxMoxVE to host vulnerable instances
- Packer & Ansible to setup vulnerable server through ProxMoxVE
- Nessus server on same subnet
- VPN that students log into for access (student:123)
- Log into Nessus server and scan the host
- Find Vulnerability
- Report Vulnerability to client (remediate maybe?)

https://www.apalrd.net/posts/2022/raspi_spice_vdi/

---

## Penetration Testing

**Description**: Students will exploit a vulnerable host from an attacker machine.

**Assignment**: 

**Deliverable**: Screenshots of the pentest lifecycle:
1. reconnaissance, scanning, vulnerability assessment, exploitation, and reporting

### Outline

---

## Log Analysis

**Description**: Use kc7 modules to teach students log analysis.

**Assignment**: Log analysis is an essential responsibility of all tiers of analysts. As an aspiring security professional, you must know how to manipulate, pivot, and correlate actions together to confidently make decisions that 

**Deliverable**: Screenshots of challenge completions (all three) & Final Incident Report (final module[they have a choice])

---
## OSINT

**Description**: Conduct open source intelligence on a faux company.

Assignment: 

Deliverable: Produce a threat model and report from the information you were able to find.



### what do I need to do:
1. research openvpn server
2. install openvpn server on raspberry pi
	1. https://www.youtube.com/watch?v=kLmbgJe1rEU
		1. Duck DNS <DONE>
			1. https://www.youtube.com/watch?v=s-66gmIHoyE
3. install proxmox on leftover computer in CFC
4. Student uses ovpn file to authenticate
5. while using the VPN they have access to proxmox
6. can log into proxmox with different user names
7. have access to two sets of VMs
	1. Nessus Server
	2. Kali Attack VM
		1. (vuln machine should be accessible but no console access)
			1. vulnhub?
8. From there, they can log into Nessus to scan the vulnerable box
9. They can also log into the kali vm to perform a penetration test on the box
