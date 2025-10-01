<h1 align="center">Expensa: Expense Tracking Platform</h1>

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
<img width="1024" height="747" alt="image" src="https://github.com/user-attachments/assets/b714fa7d-5ac0-4cc5-95be-958dad38f1d0" />


- User feeds in an Image of the reciept, creating an object
- When an object is created in **s3** it triggers an event notification.
- Which then triggers a **Lambda** function to create an expense record.
- This expense record is created by feeding it to **Gemini Vision Model API**, which returns the reciept data.
- The expense record is then stored in a **RDS** running on postgreeSQL.
- The backend is run on an **EC2** instance , which registers an user ,create expense record ,uploads  reciept image to a S3.
- All of these services are run using **Docker** containers to ensure availability and performance.

