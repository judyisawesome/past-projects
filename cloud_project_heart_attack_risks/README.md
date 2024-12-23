
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

---

## **Folder Structure**
The project is organized in the subfolder `Cloud_Eng_Project-main`:
- **[Cloud_Eng_Project-main/EDA.ipynb](Cloud_Eng_Project-main/EDA.ipynb)**: Exploratory Data Analysis.
- **[Cloud_Eng_Project-main/model_training.py](Cloud_Eng_Project-main/model_training.py)**: Model building and training script.
- **[Cloud_Eng_Project-main/pipeline.py](Cloud_Eng_Project-main/pipeline.py)**: Modular pipeline for preprocessing and prediction.
- **[Cloud_Eng_Project-main/requirements.txt](Cloud_Eng_Project-main/requirements.txt)**: Dependency management.

---

## **System Architecture**
The system is designed with the following components:
1. **Data Collection**: Pulled raw data from S3.
2. **Processing Pipeline**: Cleaned, transformed, and split data into train/test sets.
3. **Model Training**: Built and optimized the Random Forest model.
4. **Deployment**: Hosted the model on AWS EC2, ensuring scalability and security.
5. **Artifact Management**: Stored trained models and logs in S3.

---

## **Cost and Scalability**
- Monthly AWS cost: **$22.83**.
- Total annual cost: **$273.96**.
- Designed for efficient scaling with minimal operational costs.

---

## **Next Steps**
1. **Web Application**:
   - Build a front-end interface to collect user input and display predictions.
2. **Expand Dataset**:
   - Include additional health metrics and global demographic data.
3. **Performance Monitoring**:
   - Set up dashboards for real-time monitoring of model performance and server usage.

---

## **Contributors**
- Sydney Li, Zhuoyan Liu, Kira Luo, Jiayue Tian, Zhiyi Zhu

This project demonstrates the integration of cloud engineering with machine learning to create a reliable, scalable, and end-to-end predictive system.
