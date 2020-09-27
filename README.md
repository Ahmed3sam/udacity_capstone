## AWS Elastic Kubernetes Service - Blue Green Deployment


This project will show you how to create you infrastructure using Cloudformation and Kubernetes (EKS)

## Project Tasks:

* Working in AWS
* Using Jenkins to implement Continuous Integration and Continuous Deployment
* Building pipelines
* Working with CloudFormation to deploy clusters
* Building Kubernetes clusters
* Building Docker containers in pipelines

## Project Requirement:

> To be able to use this CI/CD pipeline you will need to install:

* Jenkins
* Blue Ocean Plugin in Jenkins
* Pipeline-AWS Plugin in Jenkins
* Docker
* AWS Cli
* Eksctl
* Kubectl


### Setting your AWS infrastructure

For deploy your infrastructure execute the next script inside cloudformation/ folder:

    sh ./create.sh CloudDevOpsCapstone network_and_eks.yml network_and_eks.json
    
Note: The creation of EKS cluster takes almost 10 minutes


## The files included are:
```sh
* /screenshot : Screenshot the result of deploy.
* /cloudformation : CloudFormation Script of Cluster Pipeline file 
* Jenkinsfile : Jenkinsfile for Creating Pipeline
* Dockerfile : Dockerfile for building the image 
* green-controller.json : Create a replication controller green pod
* green-service.json : Create the green service
* blue-controller.json : Create a replication controller blue pod
* blue-service.json : Create the blue service
* index.html : Web site Index file.
```