
# **Cloud Engineering Project: Heart Attack Risk Prediction**

This project is a **full-stack application** that predicts heart attack risks using a machine learning model deployed on AWS. The project integrates multiple stages, including data preprocessing, model building, deployment, and monitoring, demonstrating a scalable and reproducible pipeline.

---

## **Project Objective**
The goal is to build a reliable and scalable system for predicting heart attack risks based on health metrics, lifestyle choices, and demographics. The system incorporates:
- Data collection and preparation
- Machine learning model training and hyperparameter tuning
- Deployment on AWS EC2
- Logging, monitoring, and configuration for reproducibility

---

## **Data Source**
- **Heart Attack Prediction Dataset** from [Kaggle](https://www.kaggle.com/datasets/iamsouravbanerjee/heart-attack-prediction-dataset):
  - Includes 35 features covering demographics, health metrics, and lifestyle choices.

---

## **Key Features**
### **1. Data Preprocessing**
- **Feature Engineering**: Selected and standardized features like cholesterol, diabetes, blood pressure, and exercise habits.
- **Imbalanced Data Handling**: Used SMOTE to generate synthetic samples for the minority class.
- **Pipeline Modularity**: Split the pipeline into 8 reusable `.py` modules.

### **2. Model Building**
- **Model Used**: Random Forest.
- **Hyperparameter Tuning**: Conducted grid search with 5-fold cross-validation.
- **Performance Optimization**:
  - Best parameters: `{'max_depth': 40, 'max_features': 5, 'min_samples_leaf': 4, 'n_estimators': 400}`.
  - Train/test split ratio: 80/20.

### **3. Deployment**
- **Hosting on AWS EC2**:
  - Launched a `t2.micro` instance and securely connected using SSH.
  - Cloned the GitHub repository and set up a Python virtual environment.
  - Deployed the pipeline, saving all artifacts to AWS S3 for scalability.

### **4. Logging and Monitoring**
- **Configuration Files**: Centralized parameters in `default-config.yaml`.
- **Logging**: Implemented three distinct logging levels.
- **Unit Testing**: Conducted happy and unhappy path testing to ensure robust execution.
- **Code Quality**: Achieved `Pylint` score of 10/10 for all Python files.


## **Contributors**
- Sydney Li, Zhuoyan Liu, Kira Luo, Jiayue Tian, Zhiyi Zhu

This project demonstrates the integration of cloud engineering with machine learning to create a reliable, scalable, and end-to-end predictive system.
