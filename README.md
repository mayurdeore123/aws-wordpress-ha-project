# aws-wordpress-ha-project
AWS Highly Available WordPress Project (Training)

## Project Overview
This project demonstrates a highly available WordPress architecture on AWS using:
•⁠  ⁠EC2 Auto Scaling
•⁠  ⁠Application Load Balancer
•⁠  ⁠Amazon RDS
•⁠  ⁠Amazon S3
•⁠  ⁠CloudFront

Screenshots are provided as proof of implementation.

## AWS Infrastructure Screenshots

	The following screenshots demonstrate the successful setup of the AWS infrastructure used in this project.

### EC2 Instance – Running WordPress
![EC2 Instance](ec2-instance.png)

### Application Load Balancer (Active)
![Application Load Balancer](application-load-balancer-active.png)

### Auto Scaling Group
![Auto Scaling Group](auto-scaling-group.png)

### Target Group (HTTP 80)
![Target Group](target-group-http-80.png)

### Amazon RDS – MySQL Database
![RDS Database](rds-database.png)

### Amazon S3 – Storage Bucket
![S3 Bucket](s3-bucket.png)

### CloudFront Distribution
![CloudFront](cloudfront.png)

## Architecture Flow

1.⁠ ⁠User accesses the WordPress website through a public URL.
2.⁠ ⁠Request is routed via Amazon CloudFront for low latency delivery.
3.⁠ ⁠CloudFront forwards dynamic requests to the Application Load Balancer.
4.⁠ ⁠ALB distributes traffic to EC2 instances in the Auto Scaling Group.
5.⁠ ⁠EC2 instances host the WordPress application.
6.⁠ ⁠WordPress connects to Amazon RDS (MySQL) for database operations.
7.⁠ ⁠Media files and static assets are stored in Amazon S3.
8.⁠ ⁠Auto Scaling ensures high availability and fault tolerance.

## AWS Services Used

•⁠  ⁠Amazon EC2 – Compute layer for WordPress
•⁠  ⁠Auto Scaling Group – High availability and scalability
•⁠  ⁠Application Load Balancer – Traffic distribution
•⁠  ⁠Target Groups – Health checks and routing
•⁠  ⁠Amazon RDS (MySQL) – Managed database service
•⁠  ⁠Amazon S3 – Media and static file storage
•⁠  ⁠Amazon CloudFront – Content delivery network
•⁠  ⁠IAM – Secure access management
•⁠  ⁠Security Groups – Network-level security

## High Availability & Fault Tolerance

•⁠  ⁠Auto Scaling Group maintains desired EC2 capacity
•⁠  ⁠ALB performs health checks and routes traffic only to healthy instances
•⁠  ⁠RDS provides managed and reliable database service
•⁠  ⁠CloudFront reduces load on backend infrastructure
•⁠  ⁠Architecture supports horizontal scaling

## Cost Optimization

•⁠  ⁠Used AWS Free Tier eligible services where applicable
•⁠  ⁠Auto Scaling prevents over-provisioning
•⁠  ⁠CloudFront reduces EC2 bandwidth usage
•⁠  ⁠Managed services reduce operational overhead

## Key Learnings

•⁠  ⁠Designed a highly available WordPress architecture on AWS
•⁠  ⁠Gained hands-on experience with ALB, ASG, RDS, S3, and CloudFront
•⁠  ⁠Understood real-world cloud scalability and fault tolerance
•⁠  ⁠Learned AWS networking, security groups, and health checks
•⁠  ⁠Improved documentation and GitHub version control skills
