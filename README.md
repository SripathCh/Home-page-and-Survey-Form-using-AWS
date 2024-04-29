###Home Page & Survey Form using AWS

## Overview
This repository contains the artifacts for Homework 1 of the Component-based Software Development course, including a static home page and a dynamic survey form hosted on AWS services. Part 1 is hosted using AWS S3, and Part 2 is deployed on an AWS EC2 instance.

## Links
- **Part 1 - Static Home Page:** [sripathcherukuri-swe645.s3-website.us-east-2.amazonaws.com](http://sripathcherukuri-swe645.s3-website.us-east-2.amazonaws.com/)
- **Part 2 - Dynamic Survey Form:** [3.133.91.79/part2/surveyform.html](https://3.133.91.79/part2/surveyform.html)

## Part 1: Static Home Page
1. Create `index.html` and `error.html`.
2. Apply a W3.CSS template to enhance the webpage design.
3. Set up an Amazon S3 bucket for hosting:
    - Ensure you have a free tier Amazon AWS account.
    - Turn off "Block all public access" in the bucket settings.
    - Enable static web hosting and upload the HTML files.
    - Configure the bucket policy using appropriate JSON code.
    - The `index.html` should display by default; `error.html` serves as a fallback.

## Part 2: Dynamic Survey Form
1. Launch a free tier eligible EC2 instance using "Tomcat Certified by Bitnami" from AWS Marketplace.
2. Configure the instance type as `t2.micro`.
3. Create and download a new key-pair for SSH access.
4. Establish an SSH connection:
    ```bash
    ssh -i filename.pem bitnami@your-public-ip-address
    ```
5. Transfer the `.war` file from your local machine to the EC2 instance:
    ```bash
    scp -i filename.pem path/to/filename.war bitnami@your-public-ip-address
    ```
6. Move the `.war` file to the `tomcat/webapps` directory on the EC2 instance:
    ```bash
    sudo mv /home/bitnami/filename.war tomcat/webapps
    ```
7. Access the survey form via the EC2 instance's public URL.

Please note: As the AWS subscription has ended, the original deployment is no longer live. The instructions above are for archival and replication purposes.
