# Assignment 2: Edge-Computing Video Analytics Case Study

## The Problem
This assignment involved analyzing a real-world "Smart City" implementation: the Liverpool Smart Pedestrians project. The goal was to understand how to track pedestrians, cyclists, and vehicles in real-time while complying with strict privacy regulations that limit access to traditional CCTV feeds.

## My Approach
I conducted a case study analysis focusing on the technical architecture of the project:
*   **Hardware Selection:** Evaluation of the **NVIDIA Jetson TX2** and its balance between power consumption and computational performance.
*   **Software Architecture:** Analysis of the **YOLO V3** (You Only Look Once) algorithm for object detection and the **SORT** algorithm for real-time tracking.
*   **Edge vs. Cloud:** Analyzing why the "Edge" paradigm was chosen to improve privacy (processing data locally) and reduce bandwidth costs.

## Results & Insights
*   **Performance:** The system achieved a mean accuracy of 69%, maintaining a processing rate of ~20 frames per second.
*   **Privacy:** By processing video on-device and only transmitting metadata (counts and timestamps), the project successfully navigated privacy concerns.
*   **Future Recommendations:** I explored how modern advancements like **YOLOv8**, **NVIDIA Jetson Orin**, and **5G integration** could resolve current bottlenecks and improve accuracy to over 90%.

## What I Learned
I learned that "Smart City" success is not just about having the best AI model, but about balancing technological capability with practical constraints like crowd density, hardware bottlenecks (CPU vs. GPU), and public trust through privacy preservation.

---
[View the Full Case Study Analysis](./A03_[CHADJONES]_ITAI_3377.pdf)
