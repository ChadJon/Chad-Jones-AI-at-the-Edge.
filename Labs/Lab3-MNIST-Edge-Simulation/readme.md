# Lab 3: MNIST Digit Recognition - Training to Edge Simulation

## Purpose
The objective of this lab was to transition a Convolutional Neural Network (CNN) from a high-level development environment (Python in VS Code) to a simulated hardware environment using **Edge Impulse**. This demonstrates the full "pipeline" of Edge AI deployment.

## Technical Workflow
1.  **Model Development:** Trained a CNN on the MNIST digit dataset using Python.
2.  **Optimization:** Converted the model into a **TensorFlow Lite (.tflite)** format, resulting in a final model size of approximately 2.7 MB.
3.  **Hardware Simulation:** Uploaded the optimized model to Edge Impulse to test performance against a **Cortex-M4F (80MHz)** target.

## Results (Simulated on Cortex-M4F)
The simulation provided critical insights into the physical footprint of the model on low-power hardware:
*   **Processing Time (Latency):** 7 ms
*   **Peak RAM Usage:** 4 KB
*   **Flash Usage:** 2.7 MB

## Challenges & Solutions
During the "Test and Validate" phase in Edge Impulse, I encountered a **"Job failed"** error. The system was incorrectly set to "Bounding boxes (Object detection)" while I was attempting a classification task. 
*   **Solution:** I manually updated the Data Acquisition tab to re-label the samples as "digit" and adjusted the dashboard configuration to "Classification." This resolved the conflict and unlocked the performance metrics.

## Learning Outcomes
This lab shifted my mindset from prioritizing "Accuracy Only" to prioritizing **Latency** and **RAM usage**. Seeing a model process a digit in just 7ms on a simulated microcontroller highlighted how optimized AI can facilitate real-time industrial applications.

---
### Deliverables
*   [Jupyter Notebook Code](./your_notebook_name.ipynb)
*   [Simulation Documentation](./L03_Simulation_Documentation.pdf)
*   [Reflective Journal](./L03_Reflective_Journal.pdf)
