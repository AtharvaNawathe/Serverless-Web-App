# Serverless Web App

This project is a serverless web application that allows users to add products via a frontend interface. The products are then stored in a DynamoDB table. The application utilizes AWS Lambda for backend logic, API Gateway for routing requests, DynamoDB for data storage, and AWS Amplify for frontend hosting and deployment.

## Project Description

This serverless web application enables users to add products through a frontend interface, which are then stored in DynamoDB. It leverages AWS Lambda for executing backend functions, API Gateway for request handling, and AWS Amplify for seamless frontend deployment and hosting.

## Architecture

The architecture of this project involves the following AWS services:
- **AWS Lambda**: Handles backend logic and interactions with DynamoDB.
- **Amazon DynamoDB**: Stores the product information.
- **Amazon API Gateway**: Serves as the endpoint for the frontend to communicate with Lambda functions.
- **AWS Amplify**: Hosts and deploys the frontend application.

## Prerequisites

Before you begin, ensure you have the following:
- An AWS account
- AWS CLI installed and configured
- Amplify CLI installed

## Setup Instructions

1. **Clone the repository**
    ```bash
    git clone https://github.com/your-repo/serverless-web-app.git
    cd serverless-web-app
    ```

2. **Install Amplify CLI**
    ```bash
    npm install -g @aws-amplify/cli
    ```

3. **Initialize Amplify in your project**
    ```bash
    amplify init
    ```

4. **Add the necessary Amplify categories**
    ```bash
    amplify add api
    amplify add auth
    amplify push
    ```

5. **Add backend logic with Lambda**
    - Navigate to the Amplify project and add a Lambda function:
    ```bash
    amplify add function
    ```

6. **Configure API Gateway**
    - Add a new API in Amplify and link it to your Lambda function:
    ```bash
    amplify update api
    ```

7. **Deploy the frontend**
    ```bash
    amplify publish
    ```

## Usage

1. Open the Amplify-hosted URL in your browser.
2. Use the provided frontend interface to add products.
3. The products will be stored in the DynamoDB table.


![Screenshot from 2024-07-08 14-32-19](https://github.com/AtharvaNawathe/Serverless-Web-App/assets/63600324/0c39ea22-a861-434b-90db-5b269cedf0eb)
![Screenshot from 2024-07-08 14-32-38](https://github.com/AtharvaNawathe/Serverless-Web-App/assets/63600324/e7fc935f-54f6-4fdc-93d0-5e2c0a08d6e1)


