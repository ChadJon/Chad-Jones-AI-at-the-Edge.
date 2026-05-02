# Lab 2: Deploying an AI Model on a Simulated Edge Device (Conceptual)

## Purpose
The goal of this lab was to map out the entire lifecycle of a Machine Learning model destined for an Edge device. This includes environment configuration, model architecture design, and the optimization process required for resource-constrained hardware.

## Key Concepts Covered
### 1. Environment Setup
I researched the foundational requirements for an ML development environment, including:
*   **Python (3.9-3.11):** The core language for AI development.
*   **TensorFlow:** The framework used for building and training neural networks.
*   **Jupyter Notebook:** The interactive environment for documenting and testing code.

### 2. Neural Network Design (MNIST)
I designed a conceptual model for the MNIST dataset (handwritten digits) with the following architecture:
*   **Input Layer:** 28x28 grayscale images (flattened).
*   **Hidden Layers:** Dense layers with ReLU activation (128 and 64 neurons).
*   **Output Layer:** Softmax activation with 10 neurons to represent digits 0-9.

### 3. Edge Optimization (TensorFlow Lite)
A critical part of this lab was understanding **Model Conversion**. I explored how to transform a standard Keras model into a `.tflite` format using:
*   **Quantization:** Reducing model size for faster inference.
*   **Interpreter Setup:** How a simulated edge device uses a "Deployment Script" to run the model without needing the full TensorFlow library.

## Challenges Faced
The main challenge was translating technical, code-based processes into clear conceptual explanations without executing the scripts. This required deep research into how TensorFlow and TensorFlow Lite interact and the limitations of edge hardware (memory and power).

## Learning Outcomes
I gained a clear understanding of the "Training vs. Inference" divide. While training happens on powerful machines (like Google Colab), inference must be optimized for the edge using the TFLite FlatBuffer format.

---
[View the Full Conceptual Report](./L02-Chad-Jones.pdf)
