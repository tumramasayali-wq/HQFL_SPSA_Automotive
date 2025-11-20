HQFL-SPSA: Noise-Resilient Hybrid Quantum Federated Learning for Edge AI

This repository contains the implementation and validation code for the Hybrid Quantum Federated Learning (HQFL) architecture, specifically engineered for robust image classification on resource-constrained, high-noise Edge devices, such as those found in autonomous vehicles.🚀 

Project Overview:
This work addresses the triple challenge of next-generation automotive AI: Computational Efficiency (via Quantum), Data Privacy (via Federated Learning), and Operational Noise (via SPSA).The project successfully synthesizes:
1.HQNN Core: A ResNet-18 encoder coupled with a 4-qubit Variational Quantum Circuit (VQC) for efficient feature compression.
2.FedAvg: A decentralized topology validated under severe Non-IID (Non-Identically Distributed) data constraints.
3.SPSA Optimizer: Integration of the Simultaneous Perturbation Stochastic Approximation optimizer for superior robustness against system noise and instability at the Edge.

🎯 Key Technical Achievement:
The primary finding is the successful optimization of the stochastic SPSA algorithm to meet demanding speed constraints:
Benchmark Accuracy (Adam): 90.20% (in 15 rounds)
Initial SPSA Accuracy: 65.55% (SPSA convergence stalled due to low step count)
Final SPSA Accuracy (Tuned): 90.30% (Achieved in 15 rounds after strategic hyperparameter tuning, proving performance parity and noise-resilience.)

This validates the HQFL-SPSA architecture as a feasible, robust, and privacy-preserving blueprint for future self-driving systems.

🛠️ Requirements & Setup
This project requires a Python environment with the following major libraries:
Pytorch (torch, torchvision)PennyLane (for the Quantum Circuit simulation)
NumPyInstallationBashpip install torch torchvision pennylane numpy
