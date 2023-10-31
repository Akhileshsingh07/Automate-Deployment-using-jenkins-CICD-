# Jenkins-Declarative-CiCd-pipeline-with-AWS-

Overview

This repository contains the source code and configuration files for a Jenkins-based CI/CD pipeline that automates the deployment of a project on Amazon Web Services (AWS). The pipeline is defined using the Jenkins Declarative Pipeline syntax, and it is designed to streamline the build, test, and deployment processes for our project.


Pipeline Structure

The Jenkins Declarative Pipeline in this project includes 4 stages and organized into several stages, including:

    Code cloning: This stage clone the source code from the Git repository.

    Build: This stage build the docker image from Dockerfile for my-notes-app.

    pushing image to Dockerhub: This stage push the docker image to dockerhub.

    Deploy: Deploy the Container in which application is stores to AWS infrastructure.

    ![Screenshot from 2023-10-31 10-40-28](https://github.com/Akhileshsingh07/Jenkins-Declarative-CiCd-pipeline-with-AWS-/assets/87457483/6e565e23-8543-4ca6-b99e-8316673273c3)



Configuration

To configure the pipeline for specific project, we need to update the pipeline script (Jenkinsfile) to match our project's requirements. we can define environment-specific variables, credentials, and AWS-specific configurations.

Usage 

To trigger the pipeline,

    we used webhooks in our version control system to trigger the pipeline on code commits.
  

Troubleshooting

for any encounter issues while using the pipeline, please refer to the error messages and logs in Jenkins for specific details. Additionally, check your AWS credentials and permissions to ensure the pipeline can interact with AWS services as expected.
