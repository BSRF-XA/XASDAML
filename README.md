# XASDAML: A Machine Learning-Based Framework for XAS Data Analysis

**XASDAML** is a machine learning-based framework designed to streamline the process of X-ray Absorption Spectroscopy (XAS) data analysis. It integrates the entire data-processing workflow—including dataset construction, data filtering, machine learning modeling, prediction, and model evaluation—into a unified platform. With XASDAML, users can efficiently analyze large-scale XAS datasets and gain deeper insights into the relationships between spectral data and material properties.

XASDAML  
├── Module 1: XAS Spectra Simulation  
├── Module 2: Structure Descriptor Simulation  
├── Module 3: Data Reconciliation  
├── Module 4: Plotting Spectra & Descriptors  
├── Module 5: Statistics of Structure Descriptors  
├── Module 6: Data Analysis  
├── Module 7: Dataset Optimization  
├── Module 8: Dataset Division  
├── Module 9: Dataset Standardization  
├── Module 10: Machine Learning Modeling  
├── Module 11: Prediction  
└── Module 12: Model Performance Evaluation  


# How to Run

Below is a brief overview of the steps to run the entire pipeline.

## Input Data
- **File**:  3D structure file  
- **File name**: `Cu-20220624.xyz`  
- **Format**: `"lammps-dump-text"`

## Module Execution Order
You may run each module in sequence (from **Module 1** to **Module 12**) as needed for your analysis.

---

## Step-by-Step Execution Guide

1. **Install Dependencies**  
   - Ensure you have **Python 3.8+** installed.  
   - Install the required packages using the provided `requirements.txt`.

2. **Run Individual Modules**  
   Depending on your workflow, you can run each module in order:
   - **Module 1**: XAS Spectra Simulation  
   - **Module 2**: Structure Descriptor Simulation  
   - …  
   - **Module 12**: Model Performance Evaluation  

3. **Obtain Outputs**  
   Each module saves its results in the `results/output/` directory, typically with a timestamped folder for easier tracking.

---

## Installation

```bash
# 1. Python Version: Python 3.8+
# 2. Install Required Packages:
pip install -r requirements.txt

numpy==1.23.5
matplotlib==3.7.5
seaborn==0.13.2
scipy==1.10.1
ase==3.22.0
scikit-learn==0.23.1
requests==2.31.0
xraylarch==0.9.76
tqdm==4.62.3
vasppy==0.7.1.0
pandas==2.0.3
tensorflow==2.9.1
joblib==1.1.1
keras==2.9.0
pydot==3.0.2
pymatgen==2023.8.10

## Sample Input and Output

### Input
- **`Cu-20220624.xyz`**: Copper 3D structure file

### Output

1. **Simulated Spectra**  
   - `results/output/xmu`  
   - `results/output/chi`

2. **Structure Descriptors**  
   - `results/output/cr`  
   - `results/output/cr` (two descriptor files)

3. **Plotting Spectra & Descriptors**  
   - `results/output/plots_20250115_1649`

4. **Statistics of Structure Descriptors**  
   - `results/output/statistics_20250115_1707`

5. **Dataset Standardization**  
   - `results/output/datasets(JmolNN)-pre-xmu-cn`

6. **Data Analysis**  
   - `results/output/Data-Analysis_20250115_1713`

7. **Model Evaluation**  
   - `results/output-ml/ml-cn-xmu-(JmolNN)/MLPmodel-20250115_1903/Pre_Analysis`



