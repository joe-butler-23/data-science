# CS818 Obesity Analysis

This repository contains my data science project developed for the CS818 Assessment. The project explores factors impacting obesity rates using a combination of exploratory data analysis, unsupervised learning (K-Means clustering with PCA), and supervised learning (decision tree analysis).

## Overview

The goal of this project is to investigate the relationships between lifestyle factors and obesity levels using a rich dataset from the UC Irvine Machine Learning Repository. The analysis includes:
- **Exploratory Data Analysis (EDA):** Understanding distributions, correlations, and potential relationships among variables.
- **Unsupervised Learning:** Applying K-Means clustering (with PCA for dimensionality reduction) to uncover latent patterns and groupings in the data.
- **Supervised Learning:** Using decision tree classification to identify key predictors of obesity and evaluate model performance under different feature selections.

The detailed report (CS818 Assessment) is available in the `docs/` folder.

## Getting Started

### Prerequisites

- Python 3.8 or later
- Jupyter Notebook or JupyterLab
- Required Python packages (listed in `requirements.txt`)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/CS818-Obesity-Analysis.git
   cd CS818-Obesity-Analysis

2. **Create and activate a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # For Windows: venv\Scripts\activate

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt

## Project Details

### Data Exploration
- **Data Overview:**  
  The dataset includes demographic, dietary, and lifestyle variables collected from participants.
- **Exploratory Data Analysis (EDA):**  
  Notebooks in the `notebooks/` folder cover data distribution plots, correlation heatmaps, and summary statistics to reveal initial insights.

### Unsupervised Analysis
- **K-Means Clustering:**  
  After data cleaning and z-score normalization, PCA was used for dimensionality reduction. The optimal number of clusters was determined using the Elbow method and Silhouette score (resulting in k=4).
- **Cluster Insights:**  
  Clusters were analyzed to identify distinctive profiles related to obesity risk factors.

### Supervised Analysis
- **Decision Tree Classification:**  
  Different decision tree models were evaluated by adjusting the feature set (e.g., excluding weight and height to focus on lifestyle factors). The final model was compared using accuracy scores and feature importance rankings.
- **Model Evaluation:**  
  Detailed analysis of performance metrics and model interpretability is provided in the corresponding notebook.

## Running the Notebooks

To explore the analysis step-by-step, open the following notebooks in your preferred Jupyter environment:

- **`notebooks/01_EDA.ipynb`**  
  This notebook provides an exploratory data analysis (EDA) of the dataset, including data distributions, correlation heatmaps, and summary statistics.

- **`notebooks/02_Clustering.ipynb`**  
  This notebook covers the unsupervised learning component where K-Means clustering is applied. It includes data preprocessing, PCA for dimensionality reduction, and methods for determining the optimal number of clusters (using the Elbow method and Silhouette score).

- **`notebooks/03_DecisionTree.ipynb`**  
  This notebook presents the supervised learning approach using decision tree classification. It details the model training, evaluation, and analysis of feature importance while experimenting with different feature sets.
