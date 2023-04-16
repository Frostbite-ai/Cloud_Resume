# Cloud_Resume
Welcome to the Cloud Resume project! This project is inspired by cloudresumechallenge.dev and aims to create a serverless resume hosting platform using various AWS services.

Table of Contents
1. Overview
2. Features
3. Architecture
4. Getting Started
5. Contributing
6. License
Overview
The Cloud Resume project enables you to host your resume on a fully serverless architecture, providing a highly scalable and cost-effective solution. This project leverages various AWS services such as API Gateway, Lambda, DynamoDB, and S3 to deliver a seamless and dynamic user experience.

Features
1. Fully serverless architecture
2. Custom domain support
3. Resume visit counter
4. Easy to update and maintain
5. Cost-effective and highly scalable
6. Secure with SSL encryption
 

Architecture

The architecture consists of the following components:

1. S3 Bucket: Stores the static assets (HTML, CSS, JavaScript) for the resume.
2. CloudFront: Acts as a content delivery network (CDN) for serving the static assets.
3. API Gateway: Provides an HTTP API endpoint for interacting with the visit counter.
4. Lambda: Handles the serverless functions for retrieving and updating the visit counter.
5. DynamoDB: Stores the visit counter data.
Getting Started
Prerequisites
AWS Account
AWS CLI installed and configured
Python 3.x
Node.js
Serverless Framework
Deployment
Clone this repository:

bash
Copy code
git clone https://github.com/Frostbite-ai/Cloud_Resume.git
cd cloud_Resume
Install dependencies:

Copy code
npm install
Update the serverless.yml file with your custom domain (optional).

Deploy the project:

Copy code
sls deploy
Once the deployment is complete, you will receive an API endpoint and a CloudFront distribution URL. Use these URLs to access your resume and the visit counter.

Updating Your Resume
To update your resume, simply replace the contents of the public folder with your updated HTML, CSS, and JavaScript files. Then, redeploy the project using sls deploy.

Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

License
MIT License