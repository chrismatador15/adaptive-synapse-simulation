# Adaptive Synapse Simulation with Probabilistic Metaplasticity

A Python simulation of a single adaptive synapse implementing probabilistic learning, forgetting, and confidence growth. This project explores adaptive concepts of metaplasticity and serves as a foundation for building hybrid neural networks.

--

## Features

- Simulates synaptic weight adaptation over time using probabilistic updates. 
- Implements gradual forgetting and confidence growth mechanisms. 
- Visualizes synaptic weight dynamics using Matplotlib.
- Provides a framework for integrating adaptive synapses into larger neural networks 

---
## Motivation

Understanding synaptic plasticity is essential in both neuroscience and artificial intelligence. This project models how a synapse adapts, learns, and stabilizes over time, demonstrating the link between biological principles and computational learning algorithms.

---

## How it Works

1. **Initialization**:
   - Random starting synaptic weight (`w`) between 0 and 1
   - Initial confidence value (`confidence = 0.5`)
2. **Input Stream**:
   - Binary spikes (1 = spike, 0 = no spike) with structured noise
3. **Update Rules**:
   - If a spike occurs: probabilistic weight update based on confidence
   - If no spike: gradual forgetting proportional to current weight
   - Confidence increases slowly over time (experience consolidation)
4. **Visualization**:
   - Evolution of synaptic weights plotted over time
5. **Reflection**:
   - Outputs final weight, confidence, and stability metric
   - Prints whether the synapse stabilized or remains plastic

---

## Requirements

- Python 3.x  
- NumPy  
- Matplotlib  

Install dependencies via:

```bash
pip install numpy matplotlib

