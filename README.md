AWS S3, EC2, and Load Balancer Setup
Overview
This project demonstrates a basic setup on AWS using S3, EC2 instances, and an Application Load Balancer. The goal is to create a secure S3 bucket, enable logging, launch EC2 instances, and route traffic through a load balancer.

Project Steps
S3 Bucket Setup

Created an S3 bucket (myzen-bucket) with public access disabled.
Uploaded static HTML template files.
Enabled server access logging to monitor bucket activity.
EC2 Instances

Launched two Ubuntu EC2 instances and installed Apache.
Configured user data to automatically start the web server and deploy files.
Application Load Balancer

Configured an Application Load Balancer to route traffic across both EC2 instances, ensuring scalability and high availability.
Logs & Monitoring
Server access logs are stored in a target S3 bucket for review, providing visibility into bucket access and modifications.

How to Run
Access the application via the load balancer's DNS name/IP, where traffic will be evenly distributed across the EC2 instances.
