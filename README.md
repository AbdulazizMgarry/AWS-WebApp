🧮 Serverless Calculator Web App (AWS Powered)
🚀 Overview
This is a fully serverless calculator web application built using core AWS services. The app allows users to perform basic arithmetic operation (exponent), and stores the calculation history in a DynamoDB table. It is securely deployed using AWS Amplify with backend logic handled by AWS Lambda.

🧰 Tech Stack (AWS Services Used)
Service	Purpose
AWS Amplify	Hosts the frontend web app with CI/CD integration
AWS Lambda	Executes backend logic (calculator operations, data persistence)
Amazon API Gateway	Exposes RESTful API endpoints to the frontend
Amazon DynamoDB	Stores user input and results for each calculation
AWS IAM	Manages permissions for Lambda to interact with DynamoDB and other services

⚙️ How It Works
Frontend is deployed via AWS Amplify, built using simple HTML.

User inputs are sent to API Gateway, which routes them to a Lambda function.

The Lambda function performs the calculation, stores the result in DynamoDB, and returns the output.

IAM policies are used to securely authorize Lambda’s access to DynamoDB.

🖼️ Architecture Diagram

 ![Image Alt](https://github.com/AbdulazizMgarry/AWS-WebApp/blob/17e949364031dcdfa09539812db7522ec2251bc1/Architecture.png)
 
[Frontend (Amplify)]
       ↓
[API Gateway] ←→ [Lambda] ←→ [DynamoDB]

✅ Features
Simple web interface for calculator operations

Serverless backend (pay only when used)

Fast, scalable, and cost-effective architecture

Data persistence with DynamoDB

Secure access via IAM roles

🔒 Security
IAM roles and least-privilege permissions were used to:

Allow Lambda to read/write to DynamoDB

Secure access to API Gateway routes
