# Midterm Project: Cybersecurity Plan for an AI-Integrated IIoT System

## Project Overview
This project involved the design and stress-testing of a comprehensive cybersecurity framework for a large-scale **Smart Factory**. The facility integrates thousands of IIoT sensors, AI-powered predictive maintenance (LSTM/GRU), and automated visual quality inspection (YOLO v8). The goal was to ensure the safety and integrity of a cyber-physical system where AI decisions directly control physical actuators.

## Technical Scope
*   **System Architecture:** Secured an environment containing 4,000+ sensors, 80 PLCs, and 20 Edge AI Inference Nodes.
*   **Threat Modeling:** Applied the **STRIDE methodology** (Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, Elevation of Privilege) combined with **MITRE ATT&CK for ICS**.
*   **Defense Strategy:** Developed a layered defense grounded in **Zero Trust**, **Defense-in-Depth**, and **Secure by Design** principles, mapped to the **NIST CSF 2.0** and **IEC 62443** standards.

## Key Vulnerabilities Identified
I identified 15 distinct vulnerabilities across the device, network, data, and AI model layers, including:
*   **V-04 (Network):** Flat OT/IT network topology allowing lateral movement.
*   **V-11 (AI Model):** Adversarial input attacks fooling CNN defect detection models.
*   **V-12 (AI Model):** Model poisoning through training data manipulation.

## Penetration Testing Simulation
I conducted simulated attacks to validate the effectiveness of the defense strategy:
*   **Credential Attacks:** Blocked brute-force attempts on PLCs using Centralized Privileged Access Management (PAM).
*   **MitM on OPC-UA:** Intercepted traffic was unreadable due to mandatory **SignAndEncrypt** security modes.
*   **Adversarial ML:** Tested the resilience of the visual inspection pipeline against pixel-level perturbations, moving from a 40% failure rate to 10% after adversarial training.

## Results & Reflections
The project proved that technical controls alone are insufficient. A resilient posture requires a combination of network segmentation (Purdue Model), cryptographic data integrity, and a security-conscious human culture. My roadmap provides a 12-week implementation plan to transition a vulnerable legacy plant into a hardened, AI-integrated facility.

---
### Deliverables
*   [Full Cybersecurity Midterm Report](./MT_Chad_Jones_ITAI_3377.pdf)
