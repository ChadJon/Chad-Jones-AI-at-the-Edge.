# Lab 4: Industrial IoT (IIoT) Protocols & Real-Time Simulation

## Purpose
The objective of this project was to design and simulate an Industrial Internet of Things (IIoT) sensor network. The lab focused on comparing three major industrial communication protocols—**MQTT**, **CoAP**, and **OPC UA**—to understand how sensor data (temperature and humidity) is transmitted and visualized in real-time.

## Protocols Explored
*   **MQTT (Message Queuing Telemetry Transport):** A lightweight, publish-subscribe protocol ideal for low-bandwidth, high-latency environments. I used the **Mosquito broker** to manage data topics.
*   **CoAP (Constrained Application Protocol):** A REST-like protocol running over UDP, optimized for resource-limited environments that require fast communication.
*   **OPC UA (Open Platform Communications Unified Architecture):** A powerful, highly structured industrial standard for secure and standardized automation communication.

## Key Technical Contributions
*   **Asynchronous Programming:** Implemented Python's `asyncio` library to handle non-blocking communication for CoAP and OPC UA.
*   **Real-Time Visualization:** Developed dynamic dashboards using **Matplotlib** to visualize streaming sensor data.
*   **Environment Management:** Established a Python virtual environment to manage specific libraries required for industrial networking.

## Challenges & Solutions
1.  **Broker Connectivity:** Faced issues linking to the MQTT broker. I resolved this by verifying port configurations and ensuring the Mosquito service was running correctly in the background.
2.  **Asynchronous Logic:** Understanding the `await/async` structure in Python was challenging. I performed a deep dive into `asyncio` documentation to properly manage the event-loop.
3.  **Visualization Freezing:** The Matplotlib dashboard initially froze during real-time updates. I fixed this by implementing `plt.pause()` and `plt.ion()` to enable non-blocking plotting.

## Learning Outcomes
This lab reinforced the importance of choosing the right protocol for the right environment. I learned that while MQTT is excellent for scalability, OPC UA provides the structure needed for complex industrial automation. My experience with real-time data flow validation through visualization will be vital for future predictive maintenance and smart manufacturing projects.

---
### Deliverables
*   [Protocol Simulation Scripts](./) (Refer to Python files in this folder)
*   [Reflective Journal](./L04_Reflective_Journal.pdf)

*   [Visit my github page for this lab](/https://github.com/ChadJon/L04_Chad-Jones_Group-8_ITAI_3377.git)
