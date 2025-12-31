# spiking-neural-networks-connectivity
Computational study of how network connectivity, sparsity, and synaptic structure influence spiking neural dynamics using the Izhikevich model.

This repository contains the code and the full paper for a supervised research project investigating how **network connectivity and synaptic structure influence population-level spiking dynamics** in neural networks. The study combines mathematical modeling, graph-based representations, and computational analysis.

## Project Overview

Neural systems exhibit rich collective dynamics that depend not only on single-neuron properties, but also on **how neurons are connected**. This project studies how variations in:

- network sparsity (connection density),
- excitatory/inhibitory synaptic scaling,
- neuron-type composition,
- synaptic weight distributions, and
- network topology (random, lattice, small-world, scale-free),

affect emergent spiking behaviour at the population level.

The work is based on the **Izhikevich spiking neuron model**, which provides a computationally efficient yet biologically plausible framework for large-scale simulations.

---

## Research Questions

The project addresses four core questions:

1. **Connectivity density**  
   How does sparsity influence synchronization, firing regularity, and variability?

2. **Synaptic strength balance**  
   How sensitive are global rhythms and firing statistics to changes in excitatory and inhibitory scaling?

3. **Cell-type composition**  
   How do different ratios of RS, FS, and LTS neurons affect spiking patterns and spectral structure?

4. **Topology and weight distribution**  
   Do network topology and synaptic weight heterogeneity meaningfully alter population-level dynamics?

---

## Methods and Model

- **Neuron model:** Izhikevich spiking neuron model (ODE-based)
- **Network size:** 100 neurons (RS, FS, LTS types)
- **Connectivity:** Controlled sparsity with multiple graph constructions
- **Topologies:** Random, lattice, small-world (Watts–Strogatz), scale-free
- **Synaptic weights:** Uniform, normal, and log-normal distributions
- **Plasticity:** Hebbian learning with Dale’s law enforced

---

## Analysis and Metrics

The simulations are analyzed using a combination of graph-theoretic and statistical tools:

- **Structural metrics:**  
  Average degree, clustering coefficient, synaptic strength statistics

- **Spiking statistics:**  
  Mean firing rate, coefficient of variation (CV)

- **Temporal structure:**  
  Raster plots and spontaneous spiking activity spectra

- **Frequency-domain analysis:**  
  Fourier power spectra to identify dominant rhythmic components

These measures allow systematic comparison across different network regimes.

---

## Key Findings (High-level)

- Increased connectivity generally promotes synchronization and regular spiking.
- Balanced excitation and inhibition stabilize firing variability under noise.
- Changes in inhibitory neuron composition modulate rhythmic power without eliminating dominant frequencies.
- After normalization, network topology has limited impact on average firing rates, but affects variability and structure in subtle ways.

Detailed results and discussion are provided in the accompanying paper.

---

## Repository Structure

