# Neocracy Travel Connect

A full-stack, serverless contact and booking web application built for Neocracy India Travel. This project enables users to explore travel destinations and submit inquiries through a highly scalable and cost-efficient cloud architecture.

## 🚀 Project Overview
The application features a responsive React frontend that allows users to submit travel queries via a contact form. The backend is entirely serverless, handling data processing, notifications, and storage without the need for manual server management.

## 🛠️ Tech Stack (AWS Services)
- **AWS S3**: Hosts the static React website.
- **AWS Lambda**: Executes backend logic using Python 3.
- **Amazon API Gateway**: Routes frontend HTTP requests to Lambda functions.
- **Amazon DynamoDB**: Provides NoSQL storage for form submissions.
- **Amazon SNS**: Sends real-time email notifications for new inquiries.
- **AWS IAM**: Manages secure permissions and roles between services.

## 🔗 Integration Details
The project is integrated using a modern serverless workflow:
1. **Frontend**: Built with **React, TypeScript, and Tailwind CSS**, using **Axios** to send POST requests.
2. **API Layer**: **API Gateway** acts as the entry point, triggering the **Lambda** function.
3. **Backend Processing**: The **Lambda** function parses incoming data, stores a record in **DynamoDB**, and simultaneously triggers an **SNS** alert to notify the administrator.
4. **Hosting**: The production build is deployed to an **S3 bucket** configured for static website hosting.
