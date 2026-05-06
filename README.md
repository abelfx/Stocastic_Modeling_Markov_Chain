# Stochastic Modeling of Customer Churn using Markov Chains

## Project Overview
This project contains a comprehensive application of Discrete-Time Markov Chains (DTMC) to model customer lifecycles and predict churn. By bridging theoretical probability modeling with real-world data science applications, this project demonstrates the mathematical foundations of stochastic processes using the **IBM Telco Customer Churn** dataset.

## Project Objectives 

- **Mathematical Foundations:** Established a memoryless, time-homogeneous transition matrix ($P$) based on real customer data.
- **State-Space Analysis:** Partitioned the state space into **Transient** classes (`Active`, `AtRisk`) and an **Absorbing** class (`Churned`).
- **Boundary Problems:** Solved linear systems to calculate the Fundamental Matrix ($N$), Mean Hitting Times ($\mu$), and Absorption Probabilities ($B$).
- **Implementation & Applications:** Simulated long-term steady-state behavior (Stationary Distribution) using concepts foundational to the PageRank algorithm.

## Dataset
I utilized the industry-standard [IBM Telco Customer Churn dataset](https://raw.githubusercontent.com/IBM/telco-customer-churn-on-icp4d/master/data/Telco-Customer-Churn.csv). 
Customers were categorized into discrete states based on their contract type and current status:
* **Active:** Customers on long-term contracts.
* **AtRisk:** Customers on month-to-month contracts (higher volatility).
* **Churned:** Customers who have left the service (Absorbing State).

## Repository Structure
* `markov_analysis.ipynb`: The core Jupyter Notebook containing all data extraction, matrix algebra, mathematical proofs, and visual simulations.
* `requirements.txt`: Python package dependencies required to run the analysis.
* `README.md`: Project documentation and mathematical overview.

## Installation & Usage
To run the Jupyter Notebook locally, ensure you have Python installed, then install the required dependencies:

```bash
# Clone the repository
git clone https://github.com/abelfx/Stocastic_Modeling_Markov_Chain.git
cd Stocastic_Modeling_Markov_Chain

# Install dependencies
pip install -r requirements.txt

# launch the Notebook
jupyter notebook stocastic_modeling_markov_chains.ipynb
