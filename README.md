# Vehicle Data Project

Welcome to the **Vehicle Data Project**, a comprehensive machine learning pipeline designed to process, analyze, and evaluate vehicle-related data using cutting-edge technologies and tools. This project showcases end-to-end ML workflow integration, cloud deployment, and CI/CD practices, making it an excellent demonstration of advanced software and machine learning engineering skills.

---

## 🚀 **Key Features**

1. **Project Setup:**
   - Scripted project structure creation using `template.py`.
   - Modularized local package management using `setup.py` and `pyproject.toml`.
   - Virtual environment setup and dependency management with `requirements.txt`.

2. **MongoDB Integration:**
   - MongoDB Atlas integration for seamless data storage.
   - Notebook-driven data ingestion and key-value transformations to DataFrames.

3. **Logging & Exception Handling:**
   - Custom logger and exception modules for error tracking and debugging.
   - Extensively tested in demo scripts.

4. **Data Pipeline:**
   - **Data Ingestion:**
     - Fetch and transform data from MongoDB to pandas DataFrame.
     - Modularized ingestion process using configuration and entity layers.
   - **Data Validation:**
     - Schema validation for dataset integrity.
     - YAML-based schema definitions.
   - **Data Transformation:**
     - Feature engineering and data transformation pipelines.
   - **Model Training:**
     - Model training modules for predictive analysis.

5. **AWS Integration:**
   - S3 bucket for model storage.
   - EC2 instance setup for hosting and deployment.
   - IAM user-based secure access management.

6. **CI/CD Pipeline:**
   - Dockerized deployment with `Dockerfile` and `.dockerignore`.
   - GitHub Actions for automated CI/CD workflows.
   - Self-hosted runner on EC2 for efficient build and deployment.

7. **Deployment:**
   - Web application deployed on EC2 instance accessible via `5000` port.
   - Interactive model training available at `/training` route.

---

## 🛠️ **Getting Started**

### **1. Project Setup**
```bash
# Create virtual environment and activate
conda create -n vehicle python=3.10 -y
conda activate vehicle

# Install dependencies
pip install -r requirements.txt

# Verify installed packages
pip list
```

### **2. MongoDB Setup**
- Sign up on [MongoDB Atlas](https://www.mongodb.com/atlas).
- Create a cluster and set up a database user.
- Add IP access (`0.0.0.0/0`) for unrestricted access.
- Obtain the connection string and save it for configuration.

### **3. Data Ingestion**
- Configure MongoDB connection in `constants.__init__.py`.
- Use notebooks for pushing data to MongoDB and retrieving it for ingestion.

### **4. AWS Setup**
- Set up an IAM user with `AdministratorAccess` policy.
- Configure access keys as environment variables.
- Create an S3 bucket for model storage.

### **5. CI/CD and Deployment**
- Configure GitHub Actions with AWS credentials.
- Set up a self-hosted runner on an EC2 instance.
- Deploy Dockerized application to EC2 and access it at `<EC2_PUBLIC_IP>:5000`.

---

## 📂 **Project Structure**
```
project/
├── src/
│   ├── configuration/
│   ├── data_access/
│   ├── entity/
│   ├── components/
│   ├── aws_storage/
│   └── utils/
├── notebook/
├── static/
├── templates/
├── setup.py
├── pyproject.toml
├── requirements.txt
└── Dockerfile
```

---

## 💻 **Tech Stack**

- **Programming Languages:** Python 3.10
- **Database:** MongoDB Atlas
- **Cloud Services:** AWS (S3, EC2, IAM)
- **Tools & Frameworks:** Docker, GitHub Actions
- **Machine Learning:** pandas, scikit-learn

---

## 🔗 **Links**
- [MongoDB Atlas](https://www.mongodb.com/atlas)
- [AWS Management Console](https://aws.amazon.com/console/)
- [GitHub Actions](https://github.com/features/actions)

---

## 👏 **Acknowledgments**
Thank you for exploring this project. It demonstrates robust engineering practices, making it a great fit for production-grade applications and a valuable addition to any portfolio.

