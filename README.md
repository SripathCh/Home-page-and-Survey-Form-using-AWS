# Home Page and Student Survey Form Using AWS

## Description
This repository was originally developed for the SWE645 course assignment and includes two main components: a static homepage and a dynamic student survey form application. The homepage was hosted on AWS S3, and the survey form was deployed on AWS EC2. Currently, the AWS subscription has ended, and the links to these resources are inactive.

## Previous Configuration
### Part 1: Static Home Page on AWS S3
- Utilized W3.CSS templates for enhanced aesthetics.
- Included an error.html page to handle availability issues.

### Part 2: Student Survey Form
- Collected personal information, campus preferences, referral sources, likelihood of recommendation, and raffle entries through a web form.
- Validated required fields and raffle entry formats.

## General Setup and Replication
If you need to set up this project again or replicate the environment, here are the general steps you would follow:

### Requirements
- An AWS account with access to S3 and EC2 services.
- Local development environment with Eclipse EE and Tomcat for initial setup and testing.

### Steps to Replicate
1. **S3 Setup for Static Hosting:**
   - Create an S3 bucket and enable static website hosting.
   - Upload the index.html and error.html files to the bucket.
   - Configure bucket permissions and policies for public access according to AWS guidelines.

2. **EC2 Setup for Dynamic Web Application:**
   - Provision an EC2 instance using the "Tomcat Certified by Bitnami" AMI from the AWS Marketplace.
   - Deploy the WAR file for the survey application.
   - Adjust the security group settings to allow HTTP and SSH traffic.

Please note: As the AWS subscription has ended, the original deployment is no longer live. The instructions above are for archival and replication purposes.
