# ResNet18-Precision-Energy-Analysis

This repository contains the code, models, and findings for a research project focused on the energy consumption and performance of a ResNet18 model implemented with three different numerical precisions: FP32, FP16, and INT8 with Quantization-Aware Training (QAT).

## 📝 Project Context

This work is part of a research project aimed at quantifying the trade-offs between model accuracy, size, inference speed, and energy consumption when using reduced-precision numerical formats. As deep learning models become more computationally expensive, understanding their energy footprint is crucial for developing sustainable and efficient AI systems ("Green AI"), especially for deployment on resource-constrained environments like edge devices.

## 🔬 Precisions Compared

We analyze the ResNet18 model implemented with the following three precisions:

1.  **FP32 (Single Precision):** The standard 32-bit floating-point format that serves as our performance and energy baseline.
2.  **FP16 (Half Precision):** A 16-bit floating-point format, implemented using PyTorch's Automatic Mixed Precision (AMP) to accelerate training and reduce memory footprint.
3.  **QAT INT8 (8-bit Integer):** An 8-bit integer format achieved through **Quantization-Aware Training (QAT)**. QAT simulates quantization effects during training, allowing the model to adapt its weights to the lower precision format and minimize the typical accuracy loss.

## 📊 Methodology

* **Model:** ResNet18
* **Dataset:** *(e.g., CIFAR-10, ImageNet, etc. - specify your dataset here)*
* **Framework:** PyTorch
* **Energy Measurement:** *(e.g., Measured using the `pyJoules` library, NVIDIA's `nvml`, an external power meter, etc. - specify your method here)*
* **Metrics:** We compare the models based on Model Size (MB), Final Test Accuracy (%), Energy per Training Epoch (Joules), Energy per Inference (mJ), and Inference Latency (ms).

## 🎓 Citing This Work

If you use the code or findings from this research project in your own work, please consider citing this repository.

