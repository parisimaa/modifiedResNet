# ECE-GY 7123 Introduction to Deep Learning Mini-Project

This is the Mini-Project for ECE-GY 7123 Introduction to Deep Learning. The goal of this mini-project is to design a modified Residual Network (ResNet) architecture with thehighest test accuracyon the CIFAR-10 image classification dataset, under the constraint that your model has no more than 5 million parameters.

---

# Contributors

* **Parisima Abdali (pa2297@nyu.edu)**
* **Karan Vora (kv2154@nyu.edu)**
* **Ajay Tibrewal (at5632@nyu.edu)**

---

### Abstract

In this project, we introduce three modified versions of the ResNet model with the primary goal of achieving high accuracy while adhering to a constraint of less than 5 million trainable parameters. To achieve this objective, we conducted extensive experiments, leveraging different parameters and techniques, including active learning rate, efficient optimizer, layer augmentation, and dropouts. We meticulously analyzed the results of our experiments, presenting the findings in this paper. The outcomes of our work may have implications for various applications where model size and computational resources are critical factors.

We proposed a custom ResNet Architecture and we implemented 3 Networks ResNetSmall, ResNetMedium and ResNetLarge,

| Network      | Number of Parameters | Convolutional Channels | Optimizers                        | Training Accuracy | Testing Accuracy |
| ------------ | -------------------- | ---------------------- | --------------------------------- | ----------------- | ---------------- |
| ResNetSmall  | 78,042               | [16, 32, 64]           | SGD + Momentum (Nesterov Enabled) | 79.18%            | 79.40%           |
| ResNetMedium | 1,228,970            | [32, 64, 128, 256]     | SGD + Momentum (Nesterov Enabled) | 91.06%            | 87.99%           |
| ResNetLarge  | 4,903,242            | [64, 128, 256, 512]    | SGD + Momentum (Nesterov Enabled) | 94.16%            | 89.66%           |

---

### System Specification

* NYU Greene HPC VM
* CPU: 8 Virtualized Cores of Intel Xeon-Platinum 8286
* GPU: Nvidia Quadro RTX 8000
* System Memory: 96 GB
* Python Version: 3.8.6
* CUDA version: v11.8
* Torch Version: 2.0.0

---
