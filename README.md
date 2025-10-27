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
