# Modeling Fairness and Accuracy: A Multi-Objective Optimization Approach

This repository contains the final project submitted for the **AIM 846: Multiobjective Machine Learning** course.

### Team Details:

* Niranjan Gopal
* Akash Sridhar

---

## Overview

The project investigates the trade-off between fairness and accuracy in machine learning models through multi-objective optimization techniques. We aim to identify Pareto-optimal solutions that balance predictive performance with fairness constraints.

## Dataset

We utilize the [Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing), which contains information about direct marketing campaigns of a Portuguese banking institution. The sensitive attribute considered for fairness evaluation is **marital**.

## Algorithms

We used the following solvers for multi-objective optimization:

* **Optuna**
* **BoTorch**

## Repository Structure

* `1_eda_preprocess.ipynb`: Data exploration and preprocessing steps
* `2_optuna.ipynb`: Hyperparameter tuning using Optuna
* `3_botorch_lr.ipynb`: Bayesian optimization for Logistic Regression
* `3_botorch_nn.ipynb`: Bayesian optimization for Neural Networks
* `3_botorch_nn2.ipynb`: Cleaned-up NN notebook with GPU/CPU workflow handling
* `3_botorch_rf.ipynb`: Bayesian optimization for Random Forest
* `4_combining_pareto_from_all_models.ipynb`: Aggregating Pareto fronts from all models
* `bank.csv`: Original dataset
* `processed_bank_marketing.csv`: Preprocessed dataset
* `each_models_pareto_results.csv`: Pareto results for individual models
* `final_pareto_front.csv`: Combined Pareto front
* `requirements.txt`: List of dependencies



## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Niranjan-GopaL/Modeling_Fairness_Accuracy_MOO_approach.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Modeling_Fairness_Accuracy_MOO_approach
   ```

3. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

Run the Jupyter notebooks in the order listed above to reproduce the results.
Ensure that the datasets are placed in the appropriate directories as referenced in the notebooks.
