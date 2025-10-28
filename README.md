# Stability and Connectivity in Directed Random Graphs

## Project Description
This project investigates the stability of strongly connected components (SCCs) and typical distances in **directed random graphs** under arc addition/removal perturbations. We simulate two graph models, **Erdős–Rényi (ER)** and **Directed Configuration Model (DCM)** across varying network sizes and densities. By measuring SCC sizes, average distances, and diameters under perturbations, we provide insights into network connectivity stability.

## Research Alignment
- **Stability and directed networks** 
- **High-dimensional, time-series, and network modeling** 
- **Probability theory, interacting particle systems, and stochastic modeling** 

## Methodology

### 1. Graph Models
- **Erdős–Rényi Directed Graphs:** Random edge formation with probability `p`.  
- **Directed Configuration Model:** Graphs generated from prescribed in-degree and out-degree sequences.

### 2. Connectivity Analysis
- Compute **strongly connected components (SCCs)** using NetworkX algorithms.  
- Measure **largest SCC size**, **average shortest path length**, and **diameter**.  

### 3. Perturbation Study
- Randomly **add or remove edges** (fractional perturbation).  
- Repeat connectivity analysis to assess **stability** across iterations.

### 4. Visualization
- **Histograms** of SCC sizes.  
- **Line plots** showing SCC size changes under perturbations.  
- **Heatmaps** for SCC size and distance stability.  
- **Side-by-side boxplots** comparing ER vs. DCM metrics.

### 5. Extended Analysis
- Loop over **graph sizes**: n = 1000, 3000, 5000.  
- Loop over **edge densities**: p = 0.001, 0.005, 0.01.  
- Quantify stability variations with size and density in **multi-panel plots**.  
- Generate **statistical summaries**: mean, standard deviation, and variance across perturbations.

## Tools
- Python ≥ 3.8  
- NetworkX  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  

## Expected Outcomes
- Quantitative understanding of **SCC size stability** under perturbations.  
- Insights on **average path length and diameter variations** across graph models.  
- Heatmaps and side-by-side visualizations highlighting **robustness of connectivity**.  
- Foundations for applications in **communication networks, epidemiology, and social networks**.

## Key Findings
- **ER graphs** tend to have larger SCCs and shorter average distances for sparse networks compared to DCM.  
- **DCM graphs** show more variability in SCC size and distance metrics under perturbations.  
- Minor edge perturbations affect connectivity differently depending on **graph density and size**.  
- Multi-size and multi-density analysis highlights thresholds and resilience patterns in directed networks.

## Inference
- Directed networks display **SCC formation thresholds** influenced by density and size.  
- Perturbation studies bridge **theoretical probability models** and **practical network design**.  
- This framework can be extended to large-scale networks in **communication, epidemiology, and social systems**.
- It also lays the groundwork for future work in stochastic network modeling and high-dimensional connectivity analysis.

---

> **Note:** The code is modular, with sections for graph generation, perturbation analysis, metric computation, and visualization.
