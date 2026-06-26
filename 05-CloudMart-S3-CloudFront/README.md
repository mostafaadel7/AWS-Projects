# 🛒 Task 05 – CloudMart: Secure & Scalable Static Web Infrastructure

## Overview

This project implements a secure and scalable static web content delivery architecture for **CloudMart** using Amazon S3, Amazon CloudFront, and Amazon CloudWatch.

---

## Architecture

```
User Request
     ↓
Amazon CloudFront (Global CDN)
     ↓
Amazon S3 Bucket (cloudmart-static)
     ↑
Amazon CloudWatch (Monitoring & Alerts)
```

---

## AWS Services Used

| Service | Role |
|---------|------|
| **Amazon S3** | Stores static website assets (HTML, CSS, JS, images) |
| **Amazon CloudFront** | Global CDN — caches content at edge locations worldwide |
| **Amazon CloudWatch** | Monitors performance, errors, and infrastructure health |

---

## Tasks Performed

### Task 1 – Create S3 Bucket
- Created bucket named `cloudmart-static`
- Selected AWS Region
- Uploaded static website assets

### Task 2 – Configure CloudFront Distribution
- Created a new CloudFront distribution
- Set S3 bucket as the origin
- Enabled HTTPS
- Configured caching and security settings

### Task 3 – Restrict Direct S3 Access
- Configured Origin Access Control (OAC)
- Updated S3 bucket policy to allow access only from CloudFront
- Verified direct S3 URLs are blocked

### Task 4 – Monitor with CloudWatch
- Set up CloudWatch dashboards
- Configured alarms for error rates and latency

---

## Key Security Feature

> Direct access to the S3 bucket is **blocked**. All traffic must go through CloudFront only.

---

## AWS Docs

- [Amazon S3](https://docs.aws.amazon.com/s3/)
- [Amazon CloudFront](https://docs.aws.amazon.com/cloudfront/)
- [Amazon CloudWatch](https://docs.aws.amazon.com/cloudwatch/)
