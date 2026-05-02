# Lab 5: IIoT Network Analysis - Age of Information (AoI)

## Purpose
This lab focused on analyzing the tradeoff between **Age of Information (AoI)**—a measure of data freshness—and network reliability in heterogeneous IIoT environments. Based on research by Farag et al. (2023), I explored how network congestion and signal quality affect the performance of real-time industrial controllers.

## Data Insights & Visualization
Through Exploratory Data Analysis (EDA), I identified several key patterns:
*   **Crowded Networks:** Found a **0.54 correlation** between the number of nodes and packet loss, confirming that device interference is a primary cause of unreliability.
*   **Congestion Spikes:** Box plots revealed significant outliers in AoI as node density increased, indicating that data can become "stale" suddenly due to random network clogging.
*   **The Signal Factor:** Analysis showed that **Capture Thresholds** are a critical variable; if a signal isn't clear enough for the receiver to "capture," AoI spikes immediately.

## Machine Learning Implementation
I attempted to predict AoI based on network settings using two different approaches:
1.  **Random Forest Regressor:** This model returned a negative R-squared (-0.55). While typically seen as a "poor" result, in this context, it accurately reflected the highly stochastic and noisy nature of network simulation data.
2.  **Deep Learning (Neural Network):** I developed a multi-output Neural Network to predict both AoI and Packet Loss Probability (PLP) simultaneously, demonstrating a more advanced approach to monitoring network health.

## Real-World Applications
I proposed two primary strategies to balance freshness and reliability:
*   **Priority Queuing:** Ensuring "deadline-oriented" traffic (alarms/emergency stops) jumps to the front of the queue.
*   **Smart Access:** Implementing back-off algorithms for nodes in crowded environments.
These strategies are essential for **Warehouse Robotics** and **Factory Safety Systems**.

---
### Deliverables
*   [Jupyter Notebook Implementation](./L07_Notebook_Chad_Jones_ITAI3377.ipynb)
*   [Network Analysis Summary Report](./IIoT Network Analysis Summary Report.pdf)
