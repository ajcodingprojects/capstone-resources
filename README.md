# Capstone Research Project: Hybrid Quantum Neural Networks (HQNNs)

**Author:** Andrew Nerud  
**Institution:** Saint John’s University  
**Major:** Computer Science and Mathematics  
**Advisor:** Dr. Michael Heroux

## Overview

This repository contains all materials, findings, and code associated with my senior capstone research project on **Hybrid Quantum Neural Networks (HQNNs)**. The research evaluates HQNNs in terms of model efficiency, parameter reduction, generalization capacity, and practical viability, with applications spanning image classification, quantum chemistry, and reinforcement learning.

## Research Focus

### 1. Survey of HQNNs
- Overview of quantum machine learning fundamentals: superposition, entanglement, variational quantum circuits (VQCs).
- Comparison between classical and hybrid quantum architectures.
- Summary of performance gains and implementation bottlenecks across fields like healthcare, NLP, and chemistry.

### 2. Experimental Benchmarking
- **Implemented a HQNN model** using PennyLane and TensorFlow on the MNIST dataset.
- Compared HQNN vs. classical CNN on:
  - Accuracy
  - Parameter count
  - Floating-point operations (FLOPs)
  - Training time
- HQNN achieved ~88% parameter reduction with comparable accuracy, but significantly higher training time due to quantum simulation overhead.

### 3. Explorations in Reinforcement Learning
- Ongoing work integrates HQNNs into a **multi-agent simulation in AirSim**, where a drone uses a quantum-enhanced model to guide a car along a path.
- Investigates HQNNs for dynamic decision-making under partial observability.

### 4. Futures & Ethical Implications
- Analyzed short-term trends: circuit cutting, parameter-shift optimization, interpretability tools like Q-LIME.
- Evaluated industry investment from IBM, Microsoft, Amazon.
- Discussed responsible deployment in sensitive sectors (e.g., healthcare, finance).

## Tools & Frameworks

- **Quantum Tools:** [PennyLane](https://pennylane.ai/), Qiskit (planned)
- **Classical ML:** TensorFlow, Keras
- **Simulation & Control:** AirSim (Unreal Engine), Python-based control panel
- **Analysis & Visualization:** Matplotlib, JSON, keras-flops

## Key Results

| Model                   | Accuracy | Params   | FLOPs     | Training Time |
|------------------------|----------|----------|-----------|----------------|
| Classical CNN (baseline) | 98.92%   | 93,322   | 5.6M      | 80.7 s         |
| HQNN (AngleEmbedding)  | 97.55%   | 11,162   | 2.0M      | 6665.6 s       |

HQNNs show **superior parameter efficiency**, offering promise for embedded systems and constrained environments, despite longer training times.

## 🔬 Future Work

- Finalize RL experiments integrating HQNNs as policy networks.
- Test HQNNs on real quantum hardware (e.g., IBM Q or AWS Ocelot).
- Explore interpretability frameworks like Q-LIME in RL settings.
- Contribute benchmarking templates for HQNN reproducibility.

## 🧠 Citation

If you reference this work, please cite:

```bibtex
@article{nerud2025hqnn,
  title={Evaluating Hybrid Quantum Neural Networks: Efficiency, Viability, and the Path Forward},
  author={Nerud, Andrew},
  journal={Capstone Research, Saint John's University},
  year={2025}
}
```
