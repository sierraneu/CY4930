# CY7900 Capstone Projects Pool (Spring 2023)
## Scenario 1: MITRE Adversary Emulation Plan

This project is intended to apply the MITRE ATT&amp;CK framework and tools to map a cyber incident and then use the Caldera tool to complete an emulation plan. Included into team's tasks is the deployment in the Cloud of a mock-up scenario that represents the system compromised in the cyberincident studied. 

As a result of the project, with the **Adversary Emulation Plan** is needed to elaborate **Threat Report** of the incident analized (including a STIX2.1 JSON representation).


## Scenario 2: OpenCTI

OpenCTI is an open source cyber threat intelligence platform (TIP). It includes a knowledge management database, data visualization, and context for observables and indicators. In this scenario you need to create an IaC infrastructure able to automatically **deploy an OpenCTI using Terraform**. 

Your OpenCTI server in the cloud needs to include (at least) 3 connectors, being one of them MITRE ATT&CK. 



## Scenario 3: Multi-antivirus

In this scenario you will need to deploy a web service that checks files for viruses and malware. In order to verify if the file contains viruses or is clean, the system should use, at least, 3 antivirus engines. Your service should receive a file through a web front end and then send it to each of the antivirus engines, collects the answers from all of them and present a final report. 

![](https://www.plantuml.com/plantuml/png/XOuz3e9048NxESMKKa32hXK5mSOZQ66CGHmCoJAO_Rc_EuKinGRBUU-RbwzplhS-p0PkLthYsIxiI-BN7Nk7erpnW66PFmiJUpnT7iJlYQdEXIeNQe0cEB8DbcMxRcA3Xxh0SJ84QrPLBGegvJ6MmHXqGyzeoGNZ7IHKjfACFAYqba7KVqHl4O3DkdXjnNNnCuhVTIBrFgaJgVP91G1TBC9ilW00)

This scenario architecture need to be deployed in the cloud using [kubernetes](https://kubernetes.io). This will ensure that the service is available ubiquitously and also that highly available. 


## Scenario 4: Challenges in adoption of PostQuatnum cryptography

[Open Quantum Safe](https://github.com/open-quantum-safe) is a modern cryptographic library in C with an included python binding, which allows to use it from python programs.`OQS` is C library for prototyping and experimenting with quantum-resistant cryptography.

Among other advantages, OQS includes *Post-Quantum* cryptographic algorithms:
+ Digital signature scheme *XMSS*
+ Key  agreement schemes *McEliece* and *NewHope*

You can read the following NIST publication to illustrate these challenges: 
[Exploring Challenges Associated with Adopting and Using Post-Quantum Cryptographic Algorithms](https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.04282021.pdf). 

## Scenario 5: Security logs monitoring system.

The project requires the cloud deployment of an enterprise architecture with a variety of endpoints consisting of: DNS/SQL/Web  Servers, Linux/WindowsMachines, and external laptops/devices connecting to the network through the internet. All those systems will include an agent to forward local logs into a centralized log collector (Osquery - Kibana is the recommended technology). Teams should not devote any resources to interfere with systems vulnerabilities. Finally, to test the system, a simple simulation of attacks should be used to trigger the logs of every system. 



