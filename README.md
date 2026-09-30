💻 Laptop Price Predictor

A Machine Learning regression project that predicts laptop prices based on laptop specifications.

The project includes a Streamlit web application and is containerized using Docker. The Docker image is published on Docker Hub so that the application can be pulled and run easily on any machine with Docker installed.

🚀 Project Links

GitHub Repository

https://github.com/hemant7102/laptop-price-predictor-regression-project

Docker Hub Repository

https://hub.docker.com/r/hemant7102/laptop

Docker Image

hemant7102/laptop:latest

📌 Project Overview

Laptop prices depend on several hardware and software specifications such as:

Brand

Laptop type

RAM

CPU

GPU

Operating System

Storage

Screen size

Weight

Display resolution

Other hardware specifications

This project uses Machine Learning regression techniques to learn the relationship between laptop specifications and their prices.

The trained model is integrated into a Streamlit web application where users can enter laptop specifications and receive an estimated laptop price.

🎯 Objectives

Perform data cleaning and preprocessing

Perform exploratory data analysis

Perform feature engineering

Train a regression model

Evaluate model performance

Build an interactive Streamlit application

Containerize the application using Docker

Publish the Docker image on Docker Hub

Manage the project using Git and GitHub

🛠️ Tech Stack

Programming

Python

Data Analysis

Pandas

NumPy

Matplotlib

Seaborn

Machine Learning

Scikit-learn

Regression

Feature Engineering

Model Evaluation

Web Application

Streamlit

MLOps / Deployment

Docker

Docker Hub

Git

GitHub

📂 Project Structure

laptop-price-predictor-regression-project/
│
├── app.py
├── laptop_data.csv
├── df.pkl
├── pipe.pkl
├── requirements.txt
├── Dockerfile
├── .dockerignore
├── Procfile
├── setup.sh
├── README.md
└── .gitignore

🔄 Machine Learning Workflow

Raw Dataset
     │
     ▼
Data Cleaning
     │
     ▼
Exploratory Data Analysis
     │
     ▼
Feature Engineering
     │
     ▼
Train / Test Split
     │
     ▼
Data Preprocessing
     │
     ▼
Regression Model
     │
     ▼
Model Evaluation
     │
     ▼
Save Model Pipeline
     │
     ▼
Streamlit Application
     │
     ▼
Docker Container
     │
     ▼
Docker Hub

🧠 Machine Learning Approach

The project uses a regression approach because laptop price is a continuous numerical target.

The trained preprocessing and model pipeline is stored in:

pipe.pkl

The project also contains:

df.pkl

which is used by the application for the required data information.

🖥️ Run the Application Locally

1. Clone the repository

git clone https://github.com/hemant7102/laptop-price-predictor-regression-project.git

2. Navigate to the project

cd laptop-price-predictor-regression-project

3. Create a virtual environment

python -m venv venv

4. Activate the environment

Windows

venv\Scripts\activate

Linux / macOS

source venv/bin/activate

5. Install dependencies

pip install -r requirements.txt

6. Run Streamlit

streamlit run app.py

Open:

http://localhost:8501

🐳 Run Using Docker

The application is containerized using Docker.

Pull the Docker image

docker pull hemant7102/laptop:latest

Run the Docker container

docker run -p 8501:8501 hemant7102/laptop:latest

Open the application:

http://localhost:8501

🏗️ Build the Docker Image Locally

To build the Docker image yourself:

docker build -t hemant7102/laptop .

Run the image:

docker run -p 8501:8501 hemant7102/laptop

📦 Docker Hub

Docker Hub repository:

https://hub.docker.com/r/hemant7102/laptop

Docker image:

hemant7102/laptop:latest

Pull the image

docker pull hemant7102/laptop:latest

Run the image

docker run -p 8501:8501 hemant7102/laptop:latest

🔧 Docker Configuration

The Dockerfile creates a reproducible environment containing:

Python

Application source code

Required dependencies

Streamlit

Machine Learning model

Configuration required to run the application

The Streamlit application runs on port:

8501

📊 Application Workflow

The Streamlit application allows users to provide laptop specifications.

Laptop Specifications
        │
        ▼
Input Data
        │
        ▼
Preprocessing Pipeline
        │
        ▼
Machine Learning Model
        │
        ▼
Predicted Laptop Price

🧪 Reproducibility

The project uses requirements.txt to define the required Python packages.

Docker provides another way to reproduce the complete application environment.

Anyone with Docker installed can run:

docker pull hemant7102/laptop:latest
docker run -p 8501:8501 hemant7102/laptop:latest

Then open:

http://localhost:8501

🚀 Future Improvements

Possible improvements include:

Hyperparameter tuning

Cross-validation

Additional feature engineering

Model comparison

SHAP-based model explainability

MLflow experiment tracking

Model versioning

CI/CD automation

Automated Docker image builds

Cloud deployment

Model monitoring

Data drift monitoring

👨‍💻 Author

Hemant Narute

Aspiring Data Scientist | Data Analyst | ML & MLOps Enthusiast

GitHub:

https://github.com/hemant7102

⭐ Project

If you find this project useful, feel free to explore the repository and experiment with the application.
