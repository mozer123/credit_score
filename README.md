# NLP Credit Score Development
DSC180A - B02 - Group 2

## Overview
This project involves developing a credit scoring model using natural language processing (NLP) techniques on transaction data. The goal is to improve credit risk assessment by analyzing transaction details and capturing insights from unstructured text data in transaction memos. For reproducibility, a subset of the data is provided.

### Data Privacy

The dataset used in this project is derived from Prism Data, which contains sensitive and proprietary information about financial transactions. Due to confidentiality agreements and privacy regulations, the full dataset cannot be shared publicly. Prism Data includes detailed financial information that, if exposed, could compromise the privacy of individuals and the intellectual property of the data provider.

To allow for reproducibility of the methods and analysis presented in this project while respecting these confidentiality constraints, we are providing a small, representative subset of 5000 rows. This subset captures the essential characteristics of the full dataset but does not reveal any sensitive or proprietary details. By working with this sample, other researchers can replicate the data preprocessing, feature engineering, and modeling steps without requiring access to the complete, confidential dataset.


### Data Access and Storage

To run this project, you’ll need to download the dataset subsets and place them in the appropriate directory as described below.

1. Download the dataset subsets:
    - **Inflow** Subset (2500 rows)
    - **Outflow** Subset (2500 rows)
2. Save these files in the project’s data directory. Your project directory should look like this:  
├── data  
│   ├── inflow_subset_2500.csv  
│   └── outflow_subset_2500.csv  
└── main_code_directory  

### Software Dependencies

To run the code, make sure you have Python installed. Install the necessary libraries by running the following command:

pip install -r requirements.txt

The requirements.txt file should contain the following libraries:

pandas  
numpy  
scikit-learn  
matplotlib  

Additional Notes
re: This library is used for regular expressions and is part of Python's standard library, so no additional installation is needed.

### Reproducing Results

To reproduce results, navigate to each directory and run the Jupyter notebooks in the specified order.

1. Set up Jupyter Notebook: If Jupyter is not installed, you can install it with:

pip install jupyter

2. Open and Run the Notebooks: From your terminal, navigate to the project folder and start Jupyter Notebook:

jupyter notebook

This will open Jupyter in your browser. Navigate to the relevant folder (e.g., 01_EDA, 02_bias_check, etc.) and open the notebook files.

3. Run Each Notebook in Order:

01_EDA: Run all cells to perform exploratory data analysis.  
02_bias_check: Run this notebook to check for any biases in the dataset.  
03_memo: Run the memo preprocessing steps.  
04_feat_engineering: Execute this notebook to perform feature engineering.  
05_LLM: Runs language model-related code if relevant.  
06_models: Train the models as specified in this notebook.  
07_income and 08_measure_inflow: Additional analysis and measurement steps.  
Each notebook should be self-contained and will reproduce the steps for data preprocessing, feature engineering, and model training as needed.

4. Saving Results: Be sure to save the notebook outputs after running each cell to capture the results.


### Directory Structure
Here’s a recommended structure for organizing the project files:
  
project-directory/  
├── 01_EDA/  
├── 02_bias_check/  
├── 03_memo/  
├── 04_feat_engineering/  
├── 05_LLM/  
├── 06_models/  
├── 07_income/  
├── 08_measure_inflow/  
├── data/  
│   ├── inflow_subset_2500.csv  
│   └── outflow_subset_2500.csv  
├── requirements.txt  
└── README.md  
