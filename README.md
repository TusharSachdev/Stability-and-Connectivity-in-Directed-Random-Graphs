# Stability and Connectivity in Directed Random Graphs

## Project Description
This project investigates the stability of strongly connected components (SCCs) and typical distances in directed random graphs under arc addition and removal perturbations. Using various random graph models, including Erdős-Rényi, directed configuration models, and scale-free networks, we simulate networks, measure SCC sizes, and analyze connectivity stability. The project explores how small changes to network structure affect connectivity, path lengths, and the robustness of the largest SCC.

## Research Alignment
- Stability and directed networks (Mariana Olvera-Cravioto)  
- High-dimensional, time-series, and network modeling (Vladas Pipiras)  
- Probability theory, interacting particle systems, and stochastic modeling (Vidyadhar G. Kulkarni)  

## Project Outcomes
- Simulation of directed random graphs under perturbations  
- Analysis of SCC size distributions before and after perturbations  
- Tracking of average shortest path lengths and graph diameters  
- Visualization of stability metrics using histograms and heatmaps  
- Comparative analysis across multiple graph models  

## Methodology
**Environment Setup:**  
- Directed random graph generation using Erdős-Rényi, scale-free, and directed configuration models  
- Graph perturbations implemented as a fraction of edge additions/removals  

**Algorithms & Analysis:**  
1. **SCC Analysis:** Compute strongly connected components and track the largest SCC size.  
2. **Graph Perturbation:** Randomly add and remove edges to test network stability.  
3. **Distance Metrics:** Calculate average shortest path lengths and diameters within the largest SCC.  
4. **Visualization:**  
   - Histograms of SCC sizes before and after perturbations  
   - Heatmaps showing SCC size distributions across multiple perturbations  
   - Side-by-side comparisons of different graph models  

**Evaluation:**  
- Stability of largest SCC sizes under repeated perturbations  
- Distribution of average path lengths and diameters as metrics of connectivity robustness  

## Results
- The largest SCC tends to remain robust under small perturbations, though some fragmentation occurs depending on graph density.  
- Average shortest path lengths and diameters of the largest SCC provide a quantitative measure of connectivity stability.  
- Comparisons across graph models show that scale-free and configuration-model networks exhibit different stability profiles than Erdős-Rényi graphs.  

## Discussion
- Directed random networks exhibit varying degrees of robustness depending on structure and edge probability.  
- Perturbation analysis highlights which networks maintain connectivity versus those that fragment easily.  
- Visualization of SCC size distributions and heatmaps provides a clear view of stability across multiple iterations.  

## Tools
- Python >=3.8  
- NetworkX  
- NumPy  
- Matplotlib  
- Seaborn  

## Inference
This project provides insight into the robustness and stability of directed networks under small perturbations. The framework can be extended to study resilience in real-world systems such as social networks, transportation networks, and communication systems. It also lays the groundwork for future work in stochastic network modeling and high-dimensional connectivity analysis.

# Stability and Connectivity in Directed Random Graphs

## Project Description
This project investigates the stability of strongly connected components (SCCs) and typical distances in **directed random graphs** under arc addition/removal perturbations. We simulate two graph models — **Erdős–Rényi (ER)** and **Directed Configuration Model (DCM)** — across varying network sizes and densities. By measuring SCC sizes, average distances, and diameters under perturbations, we provide insights into network connectivity stability.

## Research Alignment
- **Stability and directed networks** (Mariana Olvera-Cravioto)  
- **High-dimensional, time-series, and network modeling** (Vladas Pipiras)  
- **Probability theory, interacting particle systems, and stochastic modeling** (Vidyadhar G. Kulkarni)  

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

---

> **Note:** The code is modular, with sections for graph generation, perturbation analysis, metric computation, and visualization.
