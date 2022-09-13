# CWRU-cybersec-Final-Project
Documentation of the Final Project from the CWRU Cybersecurity course.

## Unit 24: Final Project README

### Unit Description

In this project, you will act as a security engineer supporting an organization's SOC infrastructure. The SOC analysts have noticed some discrepancies with alerting in the Kibana system and the manager has asked the security engineering team to investigate and confirm that newly created alerts are working. 

If the alerts are working, you will then monitor live traffic on the wire to detect any abnormalities that aren't reflected in the alerting system. Then, you will report back your findings to the manager with appropriate analysis.


### Unit Objectives 

<details>
    <summary>Click here to view the daily unit objectives.</summary>

  <br>

- **Days 1 and 2:** Alert and Attacking Target 1

    - Configure alerts in Kibana 
    - Attack a machine on the network.
    - Capture the flag on the victim machine.

- **Day 3:** Wireshark Strikes Back

    - Capture network traffic
    - Investigate a number of suspicious activities
    - Collect corporate misuse evidence
    - Work in groups to create a presentation


- **Day 4:** Final Group Presentations

    - Complete and submit group presentations
    - Submit an offensive red team analysis
    - Submit a defensive blue team analysis
    - Submit a network forensic analysis. 

</details>


### Lab Environment


<details><summary>Lab Details</summary>
<br>

In this unit, you will be using a new Web Vulns lab environment located in Windows Azure Lab Services. RDP into the **Windows RDP host machine** using the following credentials:

  - Username: `azadmin`
  - Password: `p4ssw0rd*`

This is a diagram of the network and the machines that will be used in this lab:

![](Images/final-project-setup.png)

Open the Hyper-V Manager to access the nested machines:

**ELK machine credentials:** The same ELK setup that you created in Project 1. It holds the Kibana dashboards.
- Username: `vagrant`
- Password: `vagrant`
- IP Address: `192.168.1.100`

**Kali:** A standard Kali Linux machine for use in the penetration test on Day 1. 
- Username: `root`
- Password: `toor`
- IP Address: `192.168.1.90`

**Capstone:** Filebeat and Metricbeat are installed and will forward logs to the ELK machine. 
- IP Address: `192.168.1.105`
   - Please note that this VM is in the network solely for the purpose of testing alerts.

**Target 1:** Exposes a vulnerable WordPress server.
- IP Address: `192.168.1.110`

**Target 2:** Students should ignore Target 2 until they have completed all other parts of the project.

</details>  

### Security+ Domains

This unit covers portions of the following domains on the Security+ exam:

- 1.0 Attacks, Threats, and Vulnerabilities 
- 2.0 Architecture and Design 
- 3.0 Implementation
- 4.0 Operations and Incident Response 

For more information about these Security+ domains, refer to the following resource: [Security+ Exam Objectives](https://comptiacdn.azureedge.net/webcontent/docs/default-source/exam-objectives/comptia-security-sy0-601-exam-objectives-(2-0).pdf?sfvrsn=8c5889ff_2)

## Final Project

Refer to the following solution files: 

### Offensive Security Summary

[Red Team: Summary of Operations](https://github.com/thunder-katz/CWRU-cybersec-Final-Project/blob/main/Red%20Team.pdf)  

### Defensive Security Summary

[Blue Team: Summary of Operations](https://github.com/thunder-katz/CWRU-cybersec-Final-Project/blob/main/Blue%20Team.pdf)  

### Network Forensics Summary

[Network Forensic Analysis Report](https://github.com/thunder-katz/CWRU-cybersec-Final-Project/blob/main/Network%20Analysis.pdf)  

## Network Topology

![Network Topology](https://github.com/thunder-katz/CWRU-cybersec-Final-Project/blob/main/Network%20Diagram.png)

The Azure Lab Environment used for this Project consists of the following machines:

| Name              	| IP Address     	| Operating System          	| Purpose                                       	|
|-------------------	|----------------	|---------------------------	|-----------------------------------------------	|
| HYPER-V Host Manager 	| 192.168.1.0/24 	| Windows 10                	| Azure Hyper-V Machine hosting Virtual Network 	|
| **Kali Linux**        	| 192.168.1.90   	| Debian Kali 5.4.0         	| Red Team Penetration (Attack) Testing Machine    	|
| _ELK Stack_         	| 192.168.1.100  	| Ubuntu 18.04.1 LTS        	| ELK Stack (Elastisearch, Logstash and Kibana)    	|
| Capstone          	| 192.168.1.105  	| Ubuntu 18.04.1 LTS         	| Vulnerable Web Server                         	|
| **Target 1**          	| 192.168.1.110  	| Debian GNU/Linux 3.2 - 4.9 	| WordPress Host                                	|
| **Target 2**          	| 192.168.1.115  	| Debian GNU/Linux 3.2 - 4.9 	| WordPress Host                                	|

### Final Group Project Submission

[Final Project - Group Presentation](https://github.com/thunder-katz/CWRU-cybersec-Final-Project/blob/main/Final%20Project%20Presentation%20-%20Group.pdf)  

---
© 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
