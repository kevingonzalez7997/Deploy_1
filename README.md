# Mannual App Deployment with ElasticBean Stalk (D1.1)
### Kevin Gonzalez 
### August 15, 2023

# Purpose

This project's purpose is to develop a URL Shortener application efficiently using Jenkins for source code management, building, and testing, and AWS Elastic Beanstalk for simplified deployment and scaling. By automating development and deployment processes, we aim to create a user-friendly URL Shortener, showcasing the power of modern DevOps practices

### Setting Up GitHub
GitHub, a prominent version control platform, is where Jenkins retrieves code through cloning. It offers essential tools for version tracking, collaborative coding, and efficient code repository management

First, create a new repository; this will serve as SCM for the application.

Next, upload the application files to the new repository.

Make sure to obtain your GitHub token for the repository you've created (Jenkins will need this later).

### IAM (Identity and Access Management)

Before you can test the code in Jenkins, ensure you set up the correct IAM permissions.

You need to configure two roles: one for Beanstalk and another for EC2.

Add AWSElasticBeanstalkWebTier, workerTier, and MulticontainerDocker as the required permissions.

This must be done before you run the code, as it controls access to resources.

### Jenkins
Jenkins, an open-source automation server, plays a crucial role in building, testing, deploying code, and distributing workloads. In this context, a dedicated node is responsible for automating the build and test steps within the infrastructure

1. Create a new item.

2. Link the new repository using the token created from Git Hub.

3. Run build if errors occur refer to troubleshooting 

### ElasticBean Stalk
1. Create an application to start.

3. Choose the platform (python 3.9).

4. Upload the zipped file from the new repository, ensuring you zip it without the parent folder.

5. Select ElasticEC2.

6. Pick the default VPC.

7. Choose the availability zone.

8. launch
![Screenshot 2023-08-15 210425](https://github.com/kevingonzalez7997/Deploy_1/assets/59447523/a4254e30-468e-44af-be62-f1d79e39c58c)
<br>
![Deployment_1_Kevin_G](https://github.com/kevingonzalez7997/Deploy_1/assets/59447523/63c46025-d6f6-42df-aeb6-fa00f2554699)
