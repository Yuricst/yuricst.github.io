---
title: "Facility Location Problem for Space-Based Assets"
excerpt: "Facility Location Problem for Space-Based Assets"
image: 
  url: '../images/flp_allocation_D1m2000.png'
  width: '291'
  height: '392'
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
toc_sticky: true
collection: project
---

## 1. Review of Facility Location Problem

The facility location problem 

The placement of facilities is a fundamental problem in terrestrial logistics. The facility location problem (FLP) is a classical problem in operations research, for which various formulations and extensions have been proposed. 
The FLP has seen a wide range of applications, including emergency services, telecommunications, healthcare, waste disposal management, and disaster response. 


## 2. Applications to space problem: on-orbit servicing depot

The problem of designing and deploying large-scale space-based architectures may be posed as an FLP. In doing so, considerations specific to space must be taken into account to successfully adapt to the application in question. 
One such application is the placement of on-orbit servicing depots. 

We consider the problem

$$
\begin{aligned}
  \min_{X,Y} \quad& \sum_{j=1} f_j Y_j + \sum_{i=1}^m \sum_{j=1}^n c_{ij} X_{ij}
  \\
  \text{such that} \quad
  & \sum_{j = 1}^n X_{ij} = 1 \quad \quad\, \forall i \in \mathcal{M}
  \\
  & X_{ij} \leq Y_j        \quad \quad \quad \,\,\,\, \forall i \in \mathcal{M}, j \in \mathcal{N}
  \\
  & X_{ij}, Y_j \in \{0, 1\} \quad \forall i \in \mathcal{M}, j \in \mathcal{N}
\end{aligned}
$$


### Related publication:

- Y. Shimane, N. Gollins, and K. Ho, “Orbital Facility Location Problem for Satellite Constellation Servicing Depots,” J. Spacecr. Rockets, pp. 1–18, Mar. 2024, doi: 10.2514/1.A35691. [https://arc.aiaa.org/doi/full/10.2514/1.A35691](https://arc.aiaa.org/doi/full/10.2514/1.A35691)

- Y. Shimane, A. Shirane, and K. Ho, “**Lunar Communication Relay Architecture Design via Multiperiod Facility Location Problem**,” 2023.

- Y. Shimane, K. Tomita, and K. Ho, “**Strategic Regions for Monitoring Incoming Low-Energy Transfers to Low-Lunar Orbits Yuri Shimane , Kento Tomita , and Koki Ho Georgia Institute of Technology**,” 2023.


### References


