# ANN_Final_Project_5
Authors: Rebecca, Ginger, Sharini, Jenna

Project Overview: This project develops machine learning models to classify breast tumors as benign or malignant using the Wisconsin Breast Cancer Diagnostic Dataset. We compare a baseline Logistic Regression model against a custom-built Neural Network to determine the most effective approach for cancer detection.

**Key Results:**
- Neural Network achieved **99.12% accuracy**
- False Negative Rate: **2.33%** (1 missed cancer case out of 43)
- Outperformed Logistic Regression baseline (97.37% accuracy)

Project Goals: 
1. Create an interpretable baseline using Logistic Regression
2. Build a multi-layer Neural Network with ReLU activation
3. Compare model performance using comprehensive metrics
4. Minimize false negatives (missing cancer cases)

Dataset: https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic

Stats:
Total samples: 569
Features: 30 (tumor cell characteristics)
Classes: Benign (357), Malignant (212)
Class balance: 62.7% benign, 37.3% malignant

Features include:
Radius, texture, perimeter, area
Smoothness, compactness, concavity
Concave points, symmetry, fractal dimension
(mean, standard error, and "worst" values for each)

Repo structure:
ANN_Final_Project_5/
├── data_exploration.ipynb          # Initial exploratory data analysis
├── data_preprocessing.ipynb        # Data cleaning
├── logistic_regression.ipynb       # Baseline model implementation
├── neural_network.ipynb            # neural network implementation
├── model_evaluation_comparison.ipynb  # model comparison
├── wdbc.data                       # Raw dataset
├── preprocessed_data.pkl           # Processed data for modeling
├── model_comparison_results.csv    # Final metrics comparison
├── evaluation_summary.pkl          # Complete evaluation results

Use "jupyter nbconvert --to python model_evaluation_comparison.ipynb --stdout | python" in terminal to run all (This notebook trains both models from scratch and compares them)

Key Findings:
Neural Network outperforms across most metrics - Achieved 99.12% accuracy vs 97.37% for Logistic Regression
Neural Network had zero false positives
Missed only 1 cancer case (2.33%) vs 2 cases (4.65%) for Logistic Regression
Clinical Significance - In cancer detection, reducing false negatives is critical


