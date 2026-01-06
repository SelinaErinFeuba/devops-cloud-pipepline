# DevOps Cloud Pipeline Web Application
This repository contains a simple web application along with the infrastructure IAC template. 
This is used to demonstrate a DevOps CI/CD pipeline on AWS.
The web application is deployed to an EC2 instance using CloudFormation.

## Repository Structure
devops-cloud-pipeline/  
├── main/  
│   ├── app/  
│      └── webapp.html         # The web application  
│   └── infrastructure/  
│       └── template.yaml       # CloudFormation template for EC2 and security group  
├── README.md                    # This file

## Deployment

1. Launch the CloudFormation stack using `main/infrastructure/template.yaml`.
2. Ensure the `MyIP` parameter matches your current IP to allow HTTP access.
3. The EC2 instance will automatically clone this repository and deploy `webapp.html` to the web server.
4. The output `WebsiteURL` will provide the URL of the deployed web application.

## References
