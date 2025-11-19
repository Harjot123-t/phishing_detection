# Phishing Detection (URL-based)

This project detects whether a URL is phishing or safe using **Machine Learning** and **Deep Learning** models. It also provides **model explainability**, **feature importance visualization**, and **risk scores** for each URL.

---

## Features

- **Dataset**: OpenML Phishing Website Dataset (ID 4534)  
- **Models**:
  - Random Forest Classifier (ML)
  - Logistic Regression (ML)
  - Support Vector Machine (ML)
  - Deep Neural Network (TensorFlow/Keras)
- **Preprocessing**: Categorical encoding + Feature scaling  
- **Evaluation**: Accuracy, Classification Report, Confusion Matrix  
- **Explainability**: SHAP plots for Random Forest & Deep Learning models  
- **Risk Scores**: Each URL gets a probability of being phishing  
- **Saved models**: 
  - `models/rf_model.pkl`  
  - `models/lr_model.pkl`  
  - `models/svm_model.pkl`  
  - `models/dl_model.h5`  
  - `models/risk_scores.csv`  

---

## Installation & Setup

1. Clone the repository:

```bash
git clone <repo_url>
cd phishing_detection

2.Create a virtual environment:
python -m venv venv

3.Activate the environment:
Windows (PowerShell):
.\venv\Scripts\Activate.ps1

4.Install required packages:
pip install -r requirements.txt

Usage
1. Open phishing_detection.ipynb in VS Code.
2. Run the notebook cells step by step:
       Load and preprocess dataset.
       Train ML models (Random Forest, Logistic Regression, SVM).
       Train Deep Learning model.
       Generate SHAP explainability plots.
       Compute and visualize risk scores.
3. All trained models and risk scores are saved in the models/ directory for future predictions.
