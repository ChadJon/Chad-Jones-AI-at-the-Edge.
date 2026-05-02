# Assignment 5: Project Blueprint - GenAI Autonomous Maintenance Agent

## Project Overview
This project serves as a comprehensive blueprint for a next-generation industrial system: the **Autonomous Maintenance Agent**. Moving beyond simple sensor alerts, this system uses Generative AI to explain *why* a machine is overheating and autonomously decide on the best course of action, such as generating maintenance tickets without human intervention.

## Technical Architecture & Design
Although this is a conceptual blueprint, it is grounded in real-world Edge AI constraints:
*   **Edge Hardware:** Designed for the **NVIDIA Jetson Orin Nano**, chosen for its ability to run local inference without a constant cloud connection.
*   **Model Selection:** Utilizes **Microsoft Phi-3**, a Small Language Model (SLM) optimized for edge deployment.
*   **Optimization:** Implements **4-bit Quantization** to ensure the model fits within the memory limits of the edge device.
*   **Communication:** Uses **MQTT (Eclipse Mosquitto)** for high-speed sensor-to-gateway data transmission and **JSON** for standardized data formatting.

## AI Reasoning & Safety
The "brain" of the agent is designed using a **Chain of Thought** reasoning style:
1.  **Input Analysis:** Monitors vibration and temperature levels.
2.  **Context Retrieval (Grounding):** Compares live data against digital machine manuals stored in local memory to prevent "hallucinations."
3.  **Decision Generation:** Translates technical anomalies into natural language maintenance suggestions.

## Security & Ethics
*   **Security:** Implements **TLS encryption** and **MAC address whitelisting** to protect the factory floor from external tampering.
*   **Ethics:** Includes a **Human-in-the-Loop** override for any action that could stop a production line, ensuring AI assists rather than replaces human oversight.

## Personal Reflection
This project taught me that the hardest part of AI is not the code, but the **architecture**. I learned that successful industrial AI requires a deep understanding of how data moves, how to keep it private at the edge, and how to optimize large models to run on small, power-efficient hardware.

---
