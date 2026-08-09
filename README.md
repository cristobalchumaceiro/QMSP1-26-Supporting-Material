# Supplementary Material

**Project Title:** Reference-Free Hygroscopic Calibration of Low-Cost IoT Networks for Forecasting Indoor Particulate Matter Exposure  
**University:** Queen Mary University of London  
**Course:** MSc Computer Science (Conversion)  
**Author:** Cristobal Chumaceiro Rangel  
**Student Number:** 160317253  
**Email:** bs16313@qmul.ac.uk  
**Supervisor:** Dr. Stefan Poslad  

---

This repository contains the supplementary material and code for the project. Below is an overview of the directory structure and environment requirements necessary to review the work.

### Important: Downloading the Data (Git LFS)
The datasets in this repository are hosted using Git Large File Storage (LFS). 
To download the data, you must install Git LFS before cloning this repository. If you download the repository as a ZIP file, the datasets will not be included.

## `/data/`
This directory contains all the datasets used and generated throughout the project, organised into a sequential pipeline:
- `01_raw/`: Original, immutable raw data files.
- `02_interim/`: Intermediate data that has been cleaned or partially processed.
- `03_calibration/`: Datasets specifically prepared for model calibration.
- `04_calibrated_master/`: The final calibrated datasets used as a master source.
- `05_forecasting/`: Datasets and features structured for the forecasting phases.
- `06_outputs/`: Final generated results, predictions, and exported datasets.

## `/notebooks/`
This folder contains the Jupyter notebooks used for data processing, analysis, and modelling. 

> **Note:** You do not need to re-run these notebooks. They have all been executed, and all cell outputs (including plots, tables, and metrics) are saved and visible directly within the notebooks for your convenience.

The notebooks are designed to be reviewed (or executed) in the following sequential order:
- `phase_0_data_preparation.ipynb`: Initial data loading, cleaning, and preparation.
- `phase_1.1_data_exploration_and_training_pool.ipynb`: Exploratory data analysis (EDA) and creation of the training pool for calibration.
- `phase_1.2_calibration_modelling_and_tuning.ipynb`: Model training, hyperparameter tuning, and calibration.
- `phase_1.3_calibration_production.ipynb`: Final execution and production of the calibrated datasets.
- `phase_2.1_forecasting_exploration.ipynb`: Exploratory analysis, setup, and modelling specifically for forecasting.
- `phase_2.2_production.ipynb`: Final forecasting execution and output generation.

## `requirements.txt`
The `requirements.txt` file lists all the Python dependencies required to execute the notebooks. Key libraries include:
- **Data Manipulation & Analysis:** `pandas`, `numpy`, `scipy`
- **Machine Learning & Modelling:** `scikit-learn`, `xgboost`, `tensorflow`
- **Visualisation:** `matplotlib`, `seaborn`
- **Environment & Utilities:** `jupyter`, `ipykernel`, `tqdm`, `joblib`

To install the dependencies, run:
```bash
pip install -r requirements.txt
```
