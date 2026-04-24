AWS Monitoring & Alerting System

Overview
This project demonstrates how to build a real-time monitoring and alerting system on AWS to detect high CPU utilization and notify stakeholders instantly.

It simulates a production-like setup where system health is continuously monitored and alerts are triggered when thresholds are exceeded.

---

Architecture
- EC2 Instance (Ubuntu)
- CloudWatch Metrics (CPU Utilization)
- CloudWatch Alarm
- SNS Topic (Email Notification)

---

 Implementation

1. EC2 Setup
- Launched Ubuntu EC2 instance
- Instance Name: `xfusion-ec2`

2. Monitoring Configuration
- Metric: CPUUtilization
- Statistic: Average
- Period: 5 minutes

 3 Alarm Setup
- Alarm Name: `xfusion-alarm`
- Threshold: >= 90%
- Evaluation Period: 1
- Action: SNS Notification

 4. Notification System
- SNS Topic: `xfusion-sns-topic`
- Sends alerts when alarm is triggered

---


 Tools Used
- AWS EC2
- AWS CloudWatch
- AWS SNS

---

Future Improvements
- Auto Scaling Group for automatic scaling
- Application Load Balancer
- CloudWatch Dashboard
- Terraform for Infrastructure as Code

---

 Outcome
A simple but effective monitoring system that improves system reliability and response time to performance issues.
