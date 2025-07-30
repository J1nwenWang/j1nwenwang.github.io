<!-- ---
layout: page
title: Research
comments: true
permalink: /project/
---

* content
{:toc}

# My Research
---

>## 1. Real-time Trusted Execution Environment <br> --- Runtime Attack Isolation
   
### Overview

A Trusted Execution Environment (TEE) is an runtime isolation solution designed to prevent security-critical code execution and data from being interfered with by potentially compromised software. Existing TEE solutions primarily focus on protecting the confidentiality and integrity of security-critical code and data, often leaving availability unprotected. However, CPSs additionally require availability, as completing tasks beyond their deadlines can lead to catastrophic consequences. This project aims to build TEEs that extend the security guarantees of existing solutions by adding availability to the existing focus on confidentiality and integrity.

* In RT-TEE [S&P 2022], we propose a real-time TEE solution that protects the confidentiality, integrity, and real-time availability of security-critical CPU tasks and sensing/actuating operations from interference by potentially compromised operating systems in real-time CPSs, leveraging ARM TrustZone.

* In AvaGPU [CCS 2023], we propose a real-time TEE solution that guarantees the confidentiality, integrity, and real-time availability of security-critical GPU tasks, safeguarding them from potentially compromised operating systems.

### Publications

* **[S&P 22]** **<u>Jinwen Wang</u>**, Ao Li, Haoran Li, Chenyang Lu, and Ning Zhang, "[RT-TEE: Real-time System Availability for Cyber-physical Systems using ARM TrustZone](https://par.nsf.gov/servlets/purl/10373878)", 43rd IEEE Symposium on Security and Privacy, 2022. *(**VehicleSec Qualcomm Best Demo Award Runner Up**)* 

* **[CCS 23]** **<u>Jinwen Wang</u>**, Yujie Wang, and Ning Zhang, "[Secure and Timely GPU Execution in Cyber-physical Systems](https://dl.acm.org/doi/pdf/10.1145/3576915.3623197)", 30th ACM Conference on Computer and Communications Security, 2023.

>## 2. Efficient Integrity and Privacy Protection <br> --- Runtime Attack Prevention
   
### Overview
   
   CPSs often have temporal or spatial constraints, such as deadlines and memory limitations. However, existing runtime information flow integrity solutions (e.g., control-flow integrity and data-flow integrity) and privacy-preserving approaches rarely consider these constraints. To address this gap, this project aims to design and implement efficient information flow integrity and privacy-preserving mechanisms to protect information integrity and privacy on CPSs without violating temporal or spatial constraints.

* In STML [DAC 2023], we propose a privacy-preserving solution that enables large DNN models to run on hardware resource-constrained microcontrollers.

* In Procrastinating CFI [RTNS 2023], we propose a control flow integrity mechanism that ensures the runtime overhead from CFI does not disrupt the schedulability of real-time CPSs.

* In OP-DFI [Security 2024], we propose a probabilistic DFI mechanism that protects the data flow integrity of real-time CPSs while minimizing the worst-case execution time (WCET) expansion, thereby reducing the impact on real-time performance.

### Publications

* **[DAC 23]** **<u>Jinwen Wang</u>**, Yuhao Wu, Han Liu, Bo Yuan, Roger Chamberlain, and Ning Zhang, "[IP Protection in TinyML](https://cybersecurity.seas.wustl.edu/paper/wang2023ip.pdf)", 60th ACM/IEEE Design Automation Conference, 2023.

* **[RTNS 23]** Tanmaya Mishra, **<u>Jinwen Wang</u>**, Thidapat Chantem, Ryan Gerdes and Ning Zhang, "[A Procrastinating Control-Flow Integrity Framework for Periodic Real-Time Systems](https://dl.acm.org/doi/pdf/10.1145/3575757.3575762)", 31st International Conference on Real-Time Networks and Systems, 2023.

* **[Security 24]** Yujie Wang, Ao Li, **<u>Jinwen Wang</u>**, Sanjoy Baruah, and Ning Zhang, "[Opportunistic Data Flow Integrity for Real-time Cyber-physical Systems Using Worst Case Execution Time Reservation](https://www.usenix.org/system/files/sec23winter-prepub-485-wang-yujie.pdf)", 33rd USENIX Security Symposium, 2024.


>## 3. Software Recovery from Memory Safety Attacks <br> --- Runtime Attack Mitigation
   
### Overview
   
   Existing runtime attack prevention mechanisms in cyber-physical systems typically halt execution upon detecting an attack to prevent further damage. However, abruptly stopping execution in CPSs can lead to catastrophic consequences. This project aims to develop a recovery mechanism that mitigates memory safety attacks while minimizing impacts on real-time performance, ensuring continuous, safe operation even under adversarial conditions.

* In Gecko[Security 2025], we propose a software recovery mechanims that recover CPS from memory safety attacks with minimized real-time performance impacts.

### Publications

* **[Security 25]** **<u>Jinwen Wang*</u>**, Ao Li*, and Ning Zhang, "[Software Availability Protection in Cyber-physical Systems](https://j1nwenwang.github.io)", 34th USENIX Security Symposium, 2025. To be appeared.

<!-- * **<u>Jinwen Wang</u>**, Yuhao Wu, Han Liu, Bo Yuan, Roger Chamberlain, and Ning Zhang, "[IP Protection in TinyML](https://cybersecurity.seas.wustl.edu/paper/wang2023ip.pdf)", 60th ACM/IEEE Design Automation Conference (**DAC**), 2023.

* Tanmaya Mishra, **<u>Jinwen Wang</u>**, Thidapat Chantem, Ryan Gerdes and Ning Zhang, "[A Procrastinating Control-Flow Integrity Framework for Periodic Real-Time Systems](https://dl.acm.org/doi/pdf/10.1145/3575757.3575762)", 31st International Conference on Real-Time Networks and Systems (**RTNS 23**), 2023.

* Yujie Wang, Ao Li, **<u>Jinwen Wang</u>**, Sanjoy Baruah, and Ning Zhang, "[Opportunistic Data Flow Integrity for Real-time Cyber-physical Systems Using Worst Case Execution Time Reservation](https://www.usenix.org/system/files/sec23winter-prepub-485-wang-yujie.pdf)", 33rd USENIX Security Symposium (**Security**), 2024. -->



---
>## 4. Attestation, Bug Discovery, and Fingerprinting <br> --- Offline Security Reasoning


### Overview
	
Offline CPS security reasoning plays an important role in reducing the attack surface in CPSs. This project aims to design and implement scalable and efficient security reasoning approaches from both pre-execution and post-execution phases.

* In Timing Bug Understanding [IROS 2022, RTAS 2024], we design and implement software tools to automatically identify and understand timing bugs in CPSs.

* In ARI [Security 2023], we propose an efficient real-time mission execution integrity attestation solution to effectively attest both runtime information flow integrity and temporal integrity after mission execution.

* In ChckUp [Security 2024], we propose an automated firmware update vulnerability discovery approach that identifies bugs in firmware update phases. Through this research, we discovered 26 zero-day vulnerabilities.

* In SIDE [Security 2025], we propose an encoding and decoding approach to embed identity information in 3D printed objects.


### Publications

* **[IROS 22]** Ao Li, Han Liu, **<u>Jinwen Wang</u>**, and Ning Zhang, "[From Timing Variations to Performance Degradation: Understanding and Mitigating the Impact of Software Execution Timing in SLAM](https://cybersecurity.seas.wustl.edu/paper/ao-iros22.pdf)", IEEE/RSJ International Conference on Intelligent Robots and Systems, 2022.

* **[Security 23]** **<u>Jinwen Wang</u>**, Yujie Wang, Ao Li, Yang Xiao, Ruide Zhang, Wenjing Lou, Y. Thomas Hou, and Ning Zhang, "[ARI: Attestation of Real-time Mission Execution Integrity](https://www.usenix.org/system/files/usenixsecurity23-wang-jinwen.pdf)", 32nd USENIX Security Symposium, 2023.

* **[RTAS 24]** Ao Li, **<u>Jinwen Wang</u>**, Sanjoy Baruah, Bruno Sinopoli, and Ning Zhang, "[An Empirical Study of Performance Interference: Timing Violation Patterns and Impacts](https://cybersecurity.seas.wustl.edu/paper/rtas24_timetrap.pdf)", 30th IEEE Real-Time and Embedded Technology and Applications Symposium, 2024.

* **[Security 24]** Yuhao Wu, **<u>Jinwen Wang</u>**, Yujie Wang, Shixuan Zhai, Zihan Li, Yi He, Kun Sun, Qi Li, and Ning Zhang, "[Your Firmware Has Arrived: A Study of Firmware Update Vulnerabilities](https://www.usenix.org/system/files/usenixsecurity24-wu-yuhao.pdf)", 33rd USENIX Security Symposium, 2024.

* **[Security 25]** **<u>Jinwen Wang*</u>**, Canran Wang*, Mi Zhou, Vinh Pham, Senyue Hao, Chao Zhou, Ning Zhang, and Netanel Raviv, "[Secure Information Embedding in Forensic 3D Fingerprinting](https://j1nwenwang.github.io)", 34th USENIX Security Symposium, 2025. To be appeared.
 -->
