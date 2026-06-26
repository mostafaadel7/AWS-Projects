# 🚀 Task 03 – Deploying with AWS App Runner

## Overview

AWS App Runner is a fully managed service that makes it easy to deploy web applications and APIs directly from source code or a container image — no infrastructure knowledge required.

---

## What I Learned

- How App Runner simplifies deployment compared to traditional methods
- How to connect App Runner to a source code or container repository
- App Runner pricing model
- How automatic deployments (CI/CD) work with App Runner

---

## Key Concepts

| Concept | Description |
|---------|-------------|
| **Source-based deployment** | App Runner builds a container from your code automatically |
| **Image-based deployment** | Deploy a pre-built container image directly |
| **Auto deployments** | Every push to your repo triggers a new deployment |
| **Provisioned instances** | Containers kept warm to ensure low latency ($0.007/GB-hour) |

---

## Tasks Performed

- Created an App Runner service
- Connected it to a source/image repository
- Configured auto-deployment settings
- Tested the deployed application URL

---

## AWS Docs

- [App Runner Documentation](https://docs.aws.amazon.com/apprunner/)
