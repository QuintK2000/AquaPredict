# 🌊 AquaPredict : Water Potability Prediction Using Machine Learning (MLOps)
This project implements a water potability prediction system using a structured MLOps pipeline, integrating MLflow, DagsHub, and DVC for experiment tracking, model versioning, and reproducibility. Multiple models, including Random Forest, Logistic Regression, and XGBoost, were evaluated, with a focus on optimizing performance through hyperparameter tuning and testing different imputation techniques for missing data. The best model is registered in the MLflow Model Registry and deployed via Streamlit cloud for real-time predictions. A Streamlit based web application provides an interactive interface for users, automatically fetching the latest registered model. 


Link: [Click here to open app]([https://example.com](https://aquapredict-saket.streamlit.app/))


## 🚀 MLOps Project Workflow

This project follows a structured workflow to streamline the MLOps process using modern tools like MLflow, DVC, and Streamlit.

### 🔄 Workflow
1. **Experiment Setup**: Use a pre-configured Cookiecutter template and initialize Git for version control.
2. **MLflow Tracking**: Log experiments and model metrics on DagsHub using MLflow.
3. **DVC Pipeline**: Set up data versioning with DVC and build a robust ML pipeline.
4. **Model Registration**: Register the best model in MLflow’s registry for easy deployment.
5. **Streamlit App**: Create a Streamlit app that fetches the latest model from MLflow and performs predictions.
6. **Deployment**: Deploy the Streamlit app on Streamlit Cloud for accessibility.

---

## 📂 Project Structure
```
📦 mlops-project
├── 📁 data
│   ├── raw
│   ├── processed
├── 📁 notebooks
├── 📁 src
│   ├── data_preprocessing.py
│   ├── train.py
│   ├── evaluate.py
│   ├── model_registry.py
│   ├── app.py
├── 📁 models
├── 📁 dvc.yaml
├── 📁 mlflow
├── 📄 requirements.txt
├── 📄 README.md
└── 📄 .gitignore
```

---

## 🔬 Experiment Tracking

### **DagsHub + MLflow**
- Log experiments on DagsHub.
- Track model metrics, parameters, and artifacts.

### **Experiment Execution**
1. **Experiment 1**: Baseline model with Random Forest.
2. **Experiment 2**: Compare multiple models (e.g., Logistic Regression, XGBoost).
3. **Experiment 3**: Test mean vs. median imputation for missing values.
4. **Experiment 4**: Hyperparameter tuning on Random Forest.

---

## 🔄 DVC Pipeline

### **Data Versioning**
- Set up DVC for versioning data on a local disk (or cloud if preferred).

### **Pipeline Stages**
1. **Data Collection**: Gather and structure data.
2. **Data Preprocessing**: Handle missing values (mean imputation).
3. **Model Building**: Train a Random Forest model.
4. **Model Evaluation**: Track performance metrics with MLflow.

---

## 📌 Model Registration

### **MLflow Registry**
- Register the best model with optimal parameters and metadata.
- Deploy the model using FastAPI or Streamlit for predictions.

---

## 🖥️ Streamlit Application

### **Streamlit App Features**
- A simple, interactive UI built with Streamlit.
- Automatically fetches the latest model from the MLflow model registry.
- Allows users to input data and receive predictions in real-time.

### **Deployment**
- The application is deployed on **Streamlit Cloud** for easy access.

---

## 🚀 Installation & Usage

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/yourusername/mlops-project.git
cd mlops-project
```

### **2️⃣ Install Dependencies**
```bash
pip install -r requirements.txt
```

### **3️⃣ Run the Streamlit App**
```bash
streamlit run src/app.py
```

### **4️⃣ (Optional) Track Experiments with MLflow**
```bash
mlflow ui
```

This will launch the MLflow tracking server at `http://localhost:5000/`.

---

## 🎯 Future Enhancements
- Implement CI/CD for automated model deployment.
- Explore additional model training pipelines.
- Add authentication to Streamlit app for secured access.

---

## 🤝 Contributing
Contributions are welcome! Feel free to fork the repo and submit a pull request.

---

## 📜 License
This project is licensed under the MIT License.

