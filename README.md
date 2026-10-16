# teens-mental-health-model

![Build Status](https://img.shields.io/badge/build-passing-brightgreen)
![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![License](https://img.shields.io/badge/license-MIT-green)

A linear regression machine learning model built within a Jupyter Notebook to analyze and predict adolescent mental health trends. By evaluating scaled datasets, this project aims to uncover correlations between various socio-demographic factors and mental well-being scores.

## Key Features
*   **Data Preprocessing:** Implements `StandardScaler` for robust data normalization and feature scaling.
*   **Linear Regression Modeling:** Utilizes a custom linear regression algorithm to predict mental health outcomes.
*   **Performance Metrics:** Evaluates model accuracy using the R-squared ($R^2$) score.
*   **Interactive Analysis:** Fully documented Jupyter Notebook (`.ipynb`) allowing step-by-step code execution and visual data exploration.

## Tech Stack
*   **Language:** Python
*   **Libraries:** Pandas, Scikit-learn (LinearRegression, StandardScaler, r2_score), NumPy, Matplotlib/Seaborn (for data visualization)
*   **Environment:** Jupyter Notebook

## Prerequisites
To run this notebook locally, ensure you have the following installed:
*   Python 3.10 or higher
*   Jupyter Notebook or JupyterLab
*   Required Python packages (listed in `requirements.txt`)

## Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/mayJver/teens-mental-health-model.git
    cd teens-mental-health-model
    ```

2.  **Create a virtual environment (Recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts ctivate`
    ```

3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  **Start Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
2.  **Open the Notebook:** Navigate to the `notebooks/` directory and open `teen_mental_health.ipynb`.
3.  **Run the Cells:** Execute the cells sequentially to observe the data loading, preprocessing, model training, and evaluation steps.

## Data Structure Overview

The model expects a CSV file containing columns such as:
*   `age`: Integer
*   `gender`: Categorical (encoded)
*   `screen_time_hours`: Float
*   `sleep_hours`: Float
*   `physical_activity_level`: Categorical (encoded)
*   `mental_health_score` (Target Variable): Float (0-100 scale)

## Results & Metrics
The current iteration of the linear regression model achieved the following performance on the test dataset:
*   **$R^2$ Score:** -0.01 
*   *In this case, the result is a negative R², indicating that there is no linear relationship between the input variables and the stress level, or that the model does not fit the data well.
Therefore, the stress level cannot be explained solely by hours of sleep, social media usage, and physical activity, suggesting that other factors are at play.
.*

