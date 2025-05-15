# DevOps CI/CD Pipeline for Java App on AWS EKS

## Project Description

This project sets up a full DevOps pipeline for a Java application using popular tools and AWS cloud. It includes:

- Storing code in GitHub  
- Building and testing the app automatically with Jenkins and Maven  
- Checking code quality with SonarQube  
- Packaging the app into Docker containers  
- Pushing Docker images to Docker Hub  
- Deploying the app on an AWS EKS Kubernetes cluster using ArgoCD for easy and automated updates  
- Creating and managing AWS infrastructure with CloudFormation templates  

This pipeline helps automate the entire process from writing code to deploying it on the cloud, making development faster and more reliable.

## How to Use

1. Clone the repository  
2. Update configuration files with your details (Docker Hub repo, AWS subnet IDs, IAM roles, etc.)  
3. Setup Jenkins and connect it with this repo  
4. Configure SonarQube and Docker Hub credentials in Jenkins  
5. Run the Jenkins pipeline to build, test, analyze, and push Docker images  
6. Deploy the app to AWS EKS using ArgoCD and Kubernetes manifests  
7. Manage AWS infrastructure with CloudFormation  

.
├── .github/
│   └── workflows/
│       └── ci.yml                   # (Optional) GitHub Actions workflow
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   └── java/
│   │   │       └── com/yourcompany/app/  # Java source code
│   │   └── test/
│   │       └── java/
│   │           └── com/yourcompany/app/  # Java test cases
│   ├── Dockerfile                   # Dockerfile to build app image
│   └── sonar-project.properties    # SonarQube configuration
├── k8s/
│   ├── deployment.yaml             # Kubernetes Deployment manifest
│   ├── service.yaml                # Kubernetes Service manifest
│   └── ingress.yaml                # (Optional) Kubernetes Ingress manifest
├── aws/
│   └── eks-cluster.yaml            # AWS CloudFormation template for EKS cluster
├── Jenkinsfile                    # Jenkins pipeline script
└── README.md                      # Project documentation


