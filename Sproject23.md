# Scenario MITRE Adversary Emulation Plan

This project is intended to apply the MITRE ATT&amp;CK methodology and tools to map a cyber incident and then use the Caldera tool to complete an emulation plan.
### Tasks
1. Understand ATT&amp;CK Framework.
2. Find the behavior—Think about the adversary’s action in a recent Cybersecurity Event
3. Research the behavior.
4. Translate the behavior into a tactic in ATT&amp;CK.
5. Elaborate an in-depth Threat Report of the incident analized (included a STIX2.1 JSON representation).
6. Elaborate an Adversary Emulation Plan using CALDERA.



# Scenario OpenCTI

OpenCTI is an open source cyber threat intelligence platform (TIP). It includes a knowledge management database, data visualization, and context for observables and indicators. In this scenario you need to create an IaC infrastructure able to automatically deploy an OpenCTI using Terraform. 

Your OpenCTI server in the cloud needs to include (at least) 3 connectors, being one of them MITRE ATT&CK. 

Your deployment need to take special care with credentials use, and it mandatory to use a Cloud-based Key managenent for them. 




# Scenario Multi-antivirus

In this scenario you will need to deploy a web service that checks files for viruses and malware. In order to verify if the file contains viruses or is clean, the system should use, at least, 3 antivirus engines. Your service should receive a file through a web front end and then send it to each of the antivirus engines, collects the answers from all of them and present a final report. 

![](https://www.plantuml.com/plantuml/png/XOuz3e9048NxESMKKa32hXK5mSOZQ66CGHmCoJAO_Rc_EuKinGRBUU-RbwzplhS-p0PkLthYsIxiI-BN7Nk7erpnW66PFmiJUpnT7iJlYQdEXIeNQe0cEB8DbcMxRcA3Xxh0SJ84QrPLBGegvJ6MmHXqGyzeoGNZ7IHKjfACFAYqba7KVqHl4O3DkdXjnNNnCuhVTIBrFgaJgVP91G1TBC9ilW00)

This scenario architecture is intended to be deployed in the cloud using [kubernetes](https://kubernetes.io). This will ensure that the service is available ubiquitously and also that highly available. 

You need to  well-known security countermeasures to protect that application in a virtual environment, but prioritize the use of containers so it can be easily deployed in almost any system.

+ FIREWALLs
+ AUDIT & LOGS 
+ COMPLIANCE 
+ MALWARE Detection (YARA, ...)
+ Public Key Infrastructure (PKI)
+ You can propose one different technology/tool but it needs to be approved by the instructor




# Scenario Performance analysis of PostQuatnum cryptographic library.

[Open Quantum Safe](https://github.com/open-quantum-safe) is a modern cryptographic library in C with an included python binding, which allows to use it from python programs.`OQS` is C library for prototyping and experimenting with quantum-resistant cryptography.

Among other advantages, OQS includes *Post-Quantum* cryptographic algorithms:
+ Digital signature scheme *XMSS*
+ Key  agreement schemes *McEliece* and *NewHope*

For organizations like the one in our scenario, change their systems towards safe postquantum cryptographic algorithms has numerous implications (storage, performance, management, ...). You can read the following NIST publication to illustrate these challenges: 
[Exploring Challenges Associated with Adopting and
Using Post-Quantum Cryptographic Algorithms](https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.04282021.pdf). 

The work in this project is to perform a complete performance analysis of this cryptographic library that shows the performance implications of the use of postquantum cryptographic algorithms for:
+ Symmetric Encryption
+ Key agreement schemes
+ Digital signature schemes
+ *Random generation, or other cryptographic mechanism can be added*

You can use well-know performance methodologies to compare currently secure algorithm and schemes versus the future algorithms to be used in the postquantum era. The following publication will provide you a guide of what performance benchmark can be used: 
[Performance analysis Paper](https://arxiv.org/pdf/2010.06139.pdf)

Finally, and only for the postquantum algorithms use you need to perform and statistical and entropy analysis of outputs based on [DieHard](https://web.archive.org/web/20160125103112/http://stat.fsu.edu/pub/diehard/) or the [NIST Randomness test](https://nvlpubs.nist.gov/nistpubs/legacy/sp/nistspecialpublication800-22r1a.pdf).





