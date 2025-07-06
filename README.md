# MLGuard for Network Traffic

**MLGuard** is an AI-powered network security system that analyzes network traffic to detect phishing and malicious behavior using machine learning. It features an end-to-end MLOps pipeline with FastAPI, MLflow, MongoDB, AWS S3, Docker, and GitHub Actions for CI/CD.

## What is This Project About?


This project is an AI-powered system that helps detect phishing and suspicious network activity. It uses machine learning models to analyze data from a network (like internet traffic) and tells you if something looks dangerous.

Even if you don't know much about AI, think of it like a smart security guard for your network — it learns from past data and keeps an eye on new traffic to catch threats before they cause harm.



##  Key Features

-  **Network Threat Detection** using Machine Learning
-  **FastAPI** with **Swagger UI** for API interaction
-  **MongoDB** for storing raw and processed data
-  **MLflow** for model tracking and metrics logging
-  **AWS S3** for model storage and backup
-  **CSV Output** for predicted results
-  **Dockerized** for easy deployment
-  **GitHub Actions** for automated CI/CD pipeline

## 🛠️ Tech Stack

- Python 
- FastAPI 
- MLflow 
- MongoDB 
- Docker 
- GitHub Actions 
- AWS S3 
- Pandas, NumPy, Scikit-learn 



## Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/mlguard-network-traffic.git
   cd mlguard-network-traffic
   ```
2. **Install Requirements**
    ```
    pip install -r requirements.txt
    ```
3. **Set Environment Variables**
    Create a .env file:
    ```
    MONGO_DB_URL="your_mongodb_connection_string"

    ```
4. **Train the Model**
    ```
    python main.py
    ```
5. **Start the FastAPI Server**
    ```
    uvicorn app:app --reload
    ```
6. **Access Swagger UI**
    ```
    http://127.0.0.1:8000/docs
    ```

## GitHub Actions CI/CD
MLGuard is configured with GitHub Actions to automate:

- Code linting

- Dependency checks

- Model retraining

- Docker image build & push

## Docker Support
```
docker build -t mlguard-app .
docker run -p 8000:8000 mlguard-app
```
## MLflow Tracking
Track model performance and experiment history:
```
mlflow ui
Visit: http://127.0.0.1:5000
```
📸 Screenshot:

## Output CSV
prediction_output/output.csv



## AWS S3 Integration
Models are automatically backed up to an S3 bucket.

📸 Screenshot:


## MongoDB Integration
Used to store:

- Raw traffic data

- Transformed feature data

- Predictions

📸 Screenshot:



## Author
Mir Sadab Ali

