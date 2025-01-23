# AWS-Projects-Repository
This repository contains various AWS projects I've worked on. Each project has its own folder with all relevant resources and documentation. 
Below are the links to the projects.

# = = = = = = = = = = = = = = = = = =   

# PROJECT 1
## Project Name: 
Three-Tier Architecture with Aurora and EC2.

## Project Link: 
https://github.com/philipessel/Deploying-Three-Tier-Architecture 

## Project Overview:
In this project, I will build a three-tier architecture in AWS. This consist of the presentation layer, the application layer, and the database layer. The architecture will be designed to be scalable, highly available, and support fault tolerance.

### •	Presentation Layer: 
A web server will serve the front end of the application using Amazon Elastic Load Balancing (ELB) to distribute traffic to multiple web servers running in Amazon EC2 Auto Scaling groups.

### •	Application Layer: 
The logic of the application will reside in an EC2 instance managed by an Auto Scaling group to handle dynamic content processing.

### •	Database Layer: 
A managed relational database, such as Amazon Aurora, will be used to store and manage application data.

This project will demonstrate how the three-tier work together to create a reliable, scalable and fault-tolerant three-tier application.  Security measures such as VPC, security groups, and IAM will be implemented to control access to resources.

# = = = = = = = = = = = = = = = = = =  

# PROJECT 2
## Project Name: 
Automated Cost Optimization for EBS Volumes and Snapshots.

## Project Link: 
https://github.com/philipessel/Cost-Optimization-for-EBS-Volumes 

## Project Overview:
This project involves the creation of a cost optimization architecture using several AWS services. It automates the identification of terminated instances and deletion of stale Elastic Block Store (EBS) volumes and their associated snapshots. The solution relies on monitoring instance states (termination) using EventBridge, monitoring volumes and Snapshots using EventBridge and Lambda, triggering automation through Lambda and notifying administrators using Amazon SNS. AWS Cost Explorer and AWS Budgets will be used to monitor and track cost savings over time.

The architecture will operate as follows:

When an instance is terminated, EventBridge will detect the instance state and trigger Lambda function to send SNS notification to admin. A second EventBridge will be scheduled to trigger another Lambda function to query EBS volumes and snapshots on weekly basis. Anytime Lambda finds an EBS volume and Snapshot that have not been attached to instance for more than 7 days (stale resources), it will delete them. This same function will then send notification to administrator about the deletion of these stale resources and then create logs of them in CloudWatch logs. AWS Cost Explorer and AWS Budgets will at the same time be used to monitor and track cost savings over time.

# = = = = = = = = = = = = = = = = = = 

# PROJECT 3
## Project Name: 
Cost Estimation and Analysis for a Three-tier Architecture.

## Project Link: 
https://github.com/philipessel/Three-Tier-Architecture-Cost-Estimate  

## Project Overview:
This project outlines the approach to calculating the estimated costs for each component of a three-tier AWS architecture. Using the AWS Pricing Calculator, I will estimate the cost of deploying the architecture over a one-month period.

The architectural diagram attached to the project illustrates all the resources included in the three-tier architecture, whose costs will be analyzed. A detailed monthly cost breakdown will be provided. This analysis will emphasize the contribution of each AWS resource to the overall cost.

Additionally, the project will identify opportunities for cost optimization and propose actionable recommendations for cost reduction.
It is important to note that this project will focus solely on cost estimation and optimization as the actual deployment of these resources had been addressed in a separate project.


# = = = = = = = = = = = = = = = = = = 

# PROJECT 4
## Project Name: 
Static Website Hosting with S3 and CloudFront.

## Project Link: 
https://github.com/philipessel/static-website-hosting-in-s3 

## Project Overview: 
In this project, I set out to host a static website using AWS services such as S3, CloudFront, and Route 53. The website will be securely delivered via CloudFront, a content delivery network (CDN), and accessed using a custom domain managed in Route 53. AWS Certificate Manager (ACM) will handle SSL certificates, ensuring the website is served over HTTPS for secure communication.
The project will be done using AWS Management Console. 

# = = = = = = = = = = = = = = = = = =  

# PROJECT 5
## Project Name: 
Using AWS Translate to Translate from English to Spanish.

## Project Link: 

https://github.com/philipessel/aws-translation-project-.git

## Project Overview:
.....


# = = = = = = = = = = = = = = = = = = 
