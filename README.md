# Predictive Maintenance Simulation for High-Energy Physics

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Status](https://img.shields.io/badge/Status-Prototype-orange)
![Focus](https://img.shields.io/badge/Focus-Reliability%20Engineering-green)

## Context
In complex industrial systems—such as the **Large Hadron Collider (LHC)**—equipment downtime is not just an inconvenience; it's a massive cost. As an **Industrial Engineering student**, I am deeply interested in how we can transition from *reactive maintenance* (fixing things when they break) to *predictive maintenance* (fixing things before they break).

## The Project
This project is a **"Digital Twin" simulation**. Since real-time LHC sensor logs are sensitive, I engineered a synthetic dataset that mimics the operational behavior of critical machinery.

### The Engineering Logic
I defined specific failure thresholds based on physical constraints:
* **Temperature Spikes (> 280K)**: Immediate critical failure risk.
* **Pressure & Vibration Interplay**: A combination of high pressure (> 13 Bar) and mechanical vibration (> 0.08mm) triggers a system warning.

## The Solution
I utilized a **Random Forest Classifier** to analyze these sensor readings. The goal was to see if the Machine Learning model could "reverse engineer" the physical rules I created without being explicitly told what they were.

### Robustness Testing
To simulate real-world sensor imperfections, I injected **stochastic noise (5%)** into the dataset. The model successfully handled this uncertainty, proving its robustness for industrial application.

##  Key Results
* The model achieved high accuracy in predicting system status.
* **Feature Importance Analysis** confirmed that the model correctly identified `Temperature` as the most critical variable, aligning perfectly with the simulated physics.

##  How to Run
1.  Clone the repository.
2.  Install dependencies: `pandas`, `numpy`, `sklearn`, `seaborn`.
3.  Run the notebook `LHC_Sensor_Predictive_Maintenance.ipynb`.

---
*Developed by Selin ADA*
*Industrial Engineering Student @ Ostim Technical University*
