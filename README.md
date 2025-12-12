# 📘 End-to-End Machine Learning Project: Student Marks Prediction

This project demonstrates an **end-to-end machine learning pipeline** that predicts student marks based on study hours.  
It covers everything from **data ingestion → model training → deployment → CI/CD on AWS** using:

- GitHub  
- AWS CodePipeline  
- AWS Elastic Beanstalk  

---

## 🚀 Project Architecture

GitHub Repository → CodePipeline → Elastic Beanstalk → Live ML App


---

## 🧠 Tech Stack

### **Machine Learning**
- Python  
- Pandas, NumPy  
- Scikit-Learn  
- Pickle (model serialization)

### **Backend**
- Flask  

### **AWS Deployment**
- AWS CodePipeline (CI/CD)  
- AWS CodeBuild (optional)  
- AWS Elastic Beanstalk  
- AWS S3  

---

## 🗂 Project Structure

ML-Projects/
├── data/
│ └── student.csv
├── src/
│ ├── components/
│ │ ├── data_ingestion.py
│ │ ├── data_transformation.py
│ │ ├── model_trainer.py
│ ├── pipeline/
│ │ ├── training_pipeline.py
│ │ └── prediction_pipeline.py
│ ├── utils.py
│ ├── exception.py
│ └── logger.py
├── templates/
│ └── index.html
├── application.py
├── requirements.txt
└── README.md


---

## 🤖 ML Pipeline Workflow

### **1️⃣ Data Ingestion**
- Loads raw dataset  
- Splits into train and test sets  
- Saves transformed data  

### **2️⃣ Data Transformation**
- Applies feature scaling  
- Handles missing values  
- Saves preprocessing pipeline  

### **3️⃣ Model Training**
- Trains multiple ML models  
- Selects best-performing model  
- Saves model as `model.pkl`  

### **4️⃣ Prediction Pipeline**
- Loads trained model  
- Accepts input from user  
- Predicts student marks  

---

## 🌐 Deployment Workflow (CI/CD on AWS)

### **1. GitHub → AWS CodePipeline**
Every Git push triggers the pipeline.

### **2. CodePipeline**
- Fetches the latest commit  
- Builds the application (optional CodeBuild)  
- Deploys to Elastic Beanstalk  

### **3. Elastic Beanstalk**
- Hosts ML web application  
- Serves the prediction model  

---

## 🛠 Run Locally

### 
1. Clone Repository**
git clone https://github.com/KartikSuryavanshi/ML-Projects.git
cd ML-Projects
2. Create Virtual Environment
conda create -n mlproject python=3.8 -y
conda activate mlproject

3. Install Dependencies
pip install -r requirements.txt

4. Start Application
python application.py

Author

Kartik Suryavanshi
GitHub: https://github.com/KartikSuryavanshi

⭐ If you find this project helpful, please star the repository! ⭐
