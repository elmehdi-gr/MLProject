# Human Activity Recognition (HAR) Project

**Course:** Machine Learning  
**Student:** G'RIGUAA El Mehdi 
**Supervisor:** Professor Fahd Kalloubi

## Overview
This project implements an end-to-end Machine Learning pipeline to recognize human activities (e.g., Walking, Sitting, Standing) using wearable IMU sensor data. It explores unsupervised clustering, classical supervised learning, and Deep Learning (CNN, MLP) approaches.

## Project Structure
```
MLProject/
├── data/
│   ├── raw/                # Original DatasetHAR files
│   └── processed/          # Preprocessed NumPy arrays and CSVs
├── notebooks/              # Jupyter notebooks for each stage
├── models/                 # Saved trained models
├── images/                 # Generated plots and visualizations
├── report/                # Project Report (.tex)
├── results/                # CSVs of model performance metrics
├── mlruns/                 # MLflow tracking data
└── requirements.txt        # Python dependencies
```

## ⚠️ Important Note on Paths
Since the project structure has been reorganized:
> [!IMPORTANT]
> **You MUST update file paths in the notebooks before running them.**
> 
> Change paths like:
> `DATA_DIR = Path('processed_data')`  
> to  
> `DATA_DIR = Path('../data/processed')`
> 
> And:
> `DATA_DIR = Path('DatasetHAR')`  
> to  
> `DATA_DIR = Path('../data/raw')`

## Getting Started

1.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

2.  **Explore Notebooks:**
    - `01_Data_Exploration.ipynb`: Initial data analysis.
    - `02_Preprocessing.ipynb`: Cleaning and formatting.
    - `06_Supervised_Models.ipynb`: Training RF, gB, SVM.
    - `08_Neural_Networks.ipynb`: Deep Learning models.

3.  **View Results:**
    - Check `report/project_report.pdf` for the detailed finding.
    - Launch MLflow to see experiment tracking:
      ```bash
      mlflow ui
      ```

## Results Summary
- **Best Model:** Random Forest & Gradient Boosting (~97% Accuracy)
- **Deep Learning:** 1D CNN performed comparably on raw data.
