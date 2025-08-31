# Developer Role Classification from Commit Footprints

## Overview
This repository contains the solution for the project "Commit Messages → Developer Role Classification." The goal is to predict a developer's role (frontend, backend, fullstack, qa) based on the data from a single code commit[cite: 813].

This project follows a professional data science workflow, including:
1.  **Exploratory Data Analysis (EDA)** to understand the dataset's properties and risks.
2.  **A Reproducible Preprocessing Pipeline** using Scikit-learn to prevent data leakage.
3.  **Modeling**, featuring a baseline, an improved model (LightGBM), and hyperparameter tuning.
4.  **Evaluation and Error Analysis** to interpret the final model's performance.

## Project Structure
- **/data/**: Contains the raw `final_dataset.csv`.
- **/notebooks/**: Contains the Jupyter notebooks for analysis and modeling.
  - `01_eda_and_preprocessing.ipynb`: The exploratory data analysis, The model training, tuning, and evaluation.
- **/reports/**: Contains the final 2-page PDF evaluation report.
- `README.md`: This file.

## How to Reproduce Results
To reproduce the results from this project end-to-end, please follow these steps:

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/Susan5504R/GDG]
    cd GDG
    ```

2.  **Create and Activate a Virtual Environment:**
    ```bash
    # Create the environment
    python -m venv venv

    # Activate it (on Windows)
    .\venv\Scripts\activate

    # Activate it (on macOS/Linux)
    source venv/bin/activate
    ```

3.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Run the Jupyter Notebooks:**
    Launch Jupyter Notebook from your terminal:
    ```bash
    jupyter notebook
    ```
    Then, open and run the notebooks in the `/notebooks/` directory `01_eda_and_preprocessing.ipynb`

## Final Model & Performance
- **Best Model:** LightGBM (Gradient Boosting)
- **Primary Metric (Macro F1 Score):** `0.9846`