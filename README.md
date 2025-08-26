# Cybersecurity Threat Detection System ☁️🔐

This project demonstrates how to build and deploy a **Cybersecurity Threat Detection System** using **Amazon SageMaker**. The system leverages **machine learning** to identify anomalous network activity that may indicate cyberattacks, such as **DDoS attacks, unauthorized access, or phishing attempts**.  

The project covers the full ML lifecycle: data ingestion, preprocessing, model training, evaluation, deployment, and real-time inference — all orchestrated with **SageMaker Pipelines**.

---

## 📊 Overview of Architecture
1. **Data Ingestion & Preprocessing**  
   - Raw network traffic logs are collected and stored in **Amazon S3**.  
   - **AWS Lambda** transforms and feature-engineers the logs into a structured dataset.  

2. **Model Training & Evaluation**  
   - An **XGBoost** model is trained in **Amazon SageMaker** to classify network activity as normal or malicious.  
   - Model artifacts are saved in **S3**.  

3. **Deployment & Inference**  
   - The trained model is deployed to a **SageMaker Endpoint** for real-time detection of security threats.  

4. **Pipeline Automation**  
   - **SageMaker Pipelines** automate preprocessing, training, and deployment.  

5. **Monitoring & Security**  
   - **Amazon CloudWatch** logs metrics and monitors endpoint performance.  
   - **AWS IAM** manages permissions and security policies across services.  

---

## 👩‍💻 Steps Performed
1. Preprocess Data and Perform Feature Engineering  
2. Train and Test the XGBoost Model  
3. Deploy the Model and Run Inference  
4. Automate the Workflow with SageMaker Pipelines  

---

## 🛠️ AWS Services Used
- **Amazon SageMaker** → Model training, deployment, and pipeline orchestration [Machine Learning]  
- **Amazon S3** → Stores raw logs, processed data, and model artifacts [Storage]  
- **AWS Lambda** → Automates preprocessing and feature extraction [Compute]  
- **Amazon CloudWatch** → Monitors metrics and model performance [Monitoring]  
- **AWS IAM** → Manages roles and permissions [Security]  

---

## 📂 Project Structure

---

## 📚 My Learnings & Contributions

- **AWS Resource Setup & Integration** – Gained hands-on experience creating and connecting different AWS services including Amazon S3, AWS Lambda, SageMaker, IAM, and CloudWatch.  
- **XGBoost & Gradient Boosting** – Learned how the XGBoost algorithm uses **gradient boosting**, where each decision tree is built sequentially to correct the errors of the previous ones.  
- **Feature Engineering** – Applied **one-hot encoding** to transform categorical features into binary columns (0/1), making them suitable for the model.  
- **Model Deployment** – Deployed and served the trained model using a **SageMaker real-time inference endpoint**.  
- **Pipeline Automation** – Set up a **SageMaker Pipeline** to automatically retrain and redeploy the model when specific conditions are met.  
- **Cost Awareness** – Gained practical understanding of the **costs associated with AWS resources** (e.g., notebooks, endpoints, S3 storage) and how to manage them efficiently to avoid unnecessary charges.  

---

## My Contributions
- Deployed the system in my own AWS account.  
- Verified the ML pipeline end-to-end (S3 → Lambda → SageMaker → Endpoint).  
- Debugged issues with endpoint creation/deletion.  
- Documented learnings about SageMaker costs and best practices. 

--- 

## Credits
This project was built by following the [ZeroToCloud](https://zerotocloud.io) program.  
All implementation steps were provided in the guide.  

---