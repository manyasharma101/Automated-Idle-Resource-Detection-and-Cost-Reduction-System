# Automated-Idle-Resource-Detection-and-Cost-Reduction-System

## Project Objective

This project automatically detects idle EC2 instances using AWS CloudWatch metrics and performs cost optimization by stopping underutilized instances.

## AWS Services Used

* Amazon EC2
* Amazon CloudWatch
* AWS Lambda
* Amazon SNS
* Amazon EventBridge
* IAM

## Workflow

1. Deploy EC2 instances.
2. Monitor CPU utilization using CloudWatch.
3. EventBridge triggers Lambda every 5 minutes.
4. Lambda checks CPU utilization.
5. If CPU usage is below 5%, Lambda stops the instance.
6. SNS sends an email notification.
7. Cloud cost is reduced by eliminating idle resources.

## Architecture

EventBridge
↓
Lambda Function
↓
CloudWatch Metrics
↓
EC2 Stop Action
↓
SNS Email Notification

## Results

* Idle EC2 instance successfully detected.
* Automatic shutdown implemented.
* Email notification sent through SNS.
* Cloud resource utilization improved.
* Operational cost reduced.

## Author
Manya Sharma
Major Project- Automated-Idle-Resource-Detection-and-Cost-Reduction-System

