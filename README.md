# Instagram Downloader WebApp

This repository contains the front-end UI and back-end infrastructure for the **Instagram Downloader** project. The application allows users to interact with AWS services to download Instagram content (e.g., stories, reels) securely. The infrastructure is provisioned using **Terraform**, and the application uses **AWS Amplify** and **API Gateway** for deployment.

---

## Features

1. **Frontend**:  
   - Web-based UI hosted on **AWS Amplify**.
   - User-friendly design for downloading Instagram content.

2. **Backend**:  
   - **AWS Lambda**: Executes the scraping logic securely.
   - **API Gateway**: Provides REST API endpoints to interact with Lambda functions.
   - **Amazon S3**: Stores downloaded content securely.

3. **Infrastructure**:  
   - **Terraform**: Fully automated setup for deploying AWS resources.
   - **IAM Policies**: Secure role-based access control for Lambda and S3.

---

## Repository Structure

```plaintext
.
├── amplify/               # Terraform files for AWS Amplify deployment
├── api_gateway/           # Terraform files for API Gateway configuration
├── lambda/                # Lambda function code and deployment files
│   ├── lambda_function.py # Python script for scraping and uploading data
│   └── lambda_package/    # Zipped package for Lambda deployment
├── s3/                    # Terraform files for S3 bucket configuration
├── iam/                   # IAM roles and policies
├── outputs/               # Terraform output configuration
├── variables/             # Terraform variables
├── main.tf                # Main Terraform configuration file
├── terraform.tfvars       # Terraform variables with user-provided values
└── README.md              # Documentation for this project


Notes
Legal Disclaimer: This project is intended for educational purposes only. Scraping Instagram or any other platform without authorization may violate their Terms of Service.
