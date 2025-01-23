<h1 align="center">Ledgerly: Expense Tracking Platform</h1>

<p align="center">
  A self-hosted, open-source platform for tracking and managing expenses.  
  Built with NextJS, Python, and AWS services, including Lambda functions and S3 storage.  
</p>

---

## Features  

### Web Application  
- Built using **NextJS** with the App Router architecture for improved navigation and performance.  
- Backend hosted on **AWS EC2**, providing scalable and reliable virtual machines.  
- Utilizes **AWS Lambda** for serverless processing with containerized functions.  
- **Amazon S3** is used for secure and efficient image storage.  

### AWS Infrastructure  
- **Amazon S3** for storing images and other files.  
- **AWS Lambda** for data processing, including handling JSON and filtering necessary information.  
- **Amazon EC2** for hosting virtual machine instances to power the application.  
- **Amazon ECR** for hosting and managing container images in a private repository.  

### External Integrations  
- **Gemini API** for extracting text from images using Google's Vision Model, within free tier limits.  
- **GitHub Actions** for implementing CI pipelines to automate build, test, and deployment processes.  

---

## Tech Stack  

- **Frontend**: NextJS   
- **Backend**: Python, FastAPI  
- **Cloud Services**: AWS (EC2, Lambda, S3, ECR)  
- **CI/CD**: GitHub Actions  
- **Containerization**: Docker  
- **Text Recognition**: Gemini API  

---

## Overview
![image](https://github.com/user-attachments/assets/6121d6e1-a9cf-4db6-8ceb-e309c16c323f)

- The **backend** consists of 3 main services being the **Python based REST API** developed using **FastAPI** for serving requests, performing CRUD operations, a **RDS Postgres** database for data storage and retrieval and a **S3 Bucket** for image storage and hosting.
- All of these services are run using **Docker** containers to ensure availability and performance.

