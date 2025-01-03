# MLOps Project

This project is designed to demonstrate a complete MLOps pipeline for a machine learning model, aiming to impress recruiters and visitors by showcasing key tools, techniques, services, and features used.

## 📦 Project Overview
The project is a Flask-based web application that allows users to:
- **Perform Single Data Point Prediction:** Using a web form.
- **Perform Batch Prediction:** Uploading CSV files for batch inference.
- **Train the Model:** Re-train the model using the web interface.

The entire pipeline is managed using MLOps best practices, including monitoring, automation, and containerization.

---

## 📂 Key Components

### 📡 Web Application
- **Framework:** Flask
- **Frontend:** HTML templates (index, form, batch, and train pages)

### 📊 Data Pipeline
- **Data Ingestion, Transformation, and Training**
- **Prediction Pipeline:** Custom prediction pipeline for both single and batch prediction.

### 🛠️ Tools & Techniques Used
- **Flask:** Web framework for deploying the model as a RESTful API.
- **Airflow:** Used for orchestrating and monitoring tasks in the pipeline: 
  - Data Ingestion
  - Data Transformation
  - Model Training
- **Docker:** For containerization and reproducibility.
- **Logging:** Implemented with a dedicated logger for better traceability.

---

## 📈 Features
- **Single Data Point Prediction:** Users can input data through a web form.
- **Batch Prediction:** Upload CSV files for batch predictions.
- **Model Training:** Retrain the model using the web interface.
- **Automated Pipelines:** Managed using Airflow and Docker.
- **Logging:** Implemented for effective debugging and monitoring.

---

## 📦 Project Structure
```
├── src
│   ├── components
│   ├── config
│   ├── logger
│   ├── pipeline
│   └── prediction
├── templates
│   ├── index.html
│   ├── form.html
│   ├── batch.html
│   └── train.html
├── batch_prediction
├── Dockerfile
├── requirements.txt
└── app.py
```

---

## 📷 Screenshots
### Single Prediction Page
![Single Prediction](https://github.com/user-attachments/assets/221e21eb-3052-40c5-af38-cf9e8300b1b2)

### Batch Prediction Page
![Batch Prediction](https://github.com/user-attachments/assets/221e21eb-3052-40c5-af38-cf9e8300b1b2)

---

## 🚀 Getting Started

### Prerequisites:
- Python 3.8+
- Docker
- Apache Airflow

### Setup:
1. **Clone the repository:**
```bash
git clone <repository-url>
cd <repository-name>
```
2. **Create a virtual environment and install dependencies:**
```bash
python -m venv env
source env/bin/activate
pip install -r requirements.txt
```
3. **Run the Flask App:**
```bash
python app.py
```
4. **Access the Web App:** Open `http://localhost:8888`

---

## 📦 Docker Integration
- Build the Docker image:
```bash
docker build -t mlops-project .
```
- Run the container:
```bash
docker run -p 8888:8888 mlops-project
```

---

## 📊 Airflow Integration
- Start the Airflow service:
```bash
airflow standalone
```
- Access Airflow at: `http://localhost:8080`

---

## 📧 Contact
- **Email:** vineetroy289@gmail.com
- **LinkedIn:** [Vineet Roy](https://linkedin.com/in/vineet-roy-0370a61a9)

---

### 📜 License
This project is licensed under the MIT License.

