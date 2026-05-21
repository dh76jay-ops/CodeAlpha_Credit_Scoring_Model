 Credit Scoring & Risk Predictor Pipeline

Enterprise-grade machine learning classification pipeline designed to quantify financial risk and predict applicant loan default probabilities. 

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Space%20Live-orange?style=flat-square)](https://huggingface.co/spaces/dh76jay-dev/CodeAlpha-Credit-Scoring-Model)
[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=flat-square)](https://www.python.org)
[![Framework](https://img.shields.io/badge/Framework-Scikit--Learn-green?style=flat-square)](https://scikit-learn.org/)

---

 Production Deployment
The predictive engine is operationalized via a Gradio web interface and hosted on cloud infrastructure.
 **[Launch Live Production Web Application](https://huggingface.co/spaces/dh76jay-dev/CodeAlpha-Credit-Scoring-Model)**

---

 Core Architecture & Features

* **Data Preprocessing:** Handled missing values, engineered financial metrics, and implemented `StandardScaler` transformations to isolate multi-scale numeric features (Age, Income, DTI).
* **Model Benchmarking:** Evaluated structural classifiers including **Logistic Regression** and **Random Forest Ensembles**.
* **Performance:** Selected model achieved optimal convergence with an empirical **ROC-AUC Score of `~0.999`**.
* **Serialization:** Exported the fitted weights and preprocessing components into a unified pipeline dictionary using Python’s `pickle` protocol for low-latency web inference.

---

 Tech Stack

| Component | Technology | Purpose |
| :--- | :--- | :--- |
| **Language** | Python | Core development stack |
| **Data Engine** | Pandas, NumPy | Feature engineering & array operations |
| **ML Framework**| Scikit-Learn | Training, scaling, and validation pipelines |
| **UI Wrapper** | Gradio | Building the user inference client |
| **Deployment** | Hugging Face Spaces | Cloud infrastructure & production hosting |

---

 Repository Structure

```text
├── Credit_Scoring_Model.ipynb   # Exploratory Data Analysis & training workbook
├── model_pipeline.pkl          # Serialized production pipeline (Scaler + Model weights)
└── README.md                   # System documentation
