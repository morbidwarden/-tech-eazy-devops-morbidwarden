## ✅ Features

- 🌐 **EC2 Instance** with Java 21 + Spring Boot App exposed on **port 80**
- 📦 **Terraform** code handles all infrastructure provisioning
- 🔐 **IAM Roles**:
  - Read-only role for log readers
  - Write-only role for the EC2 app instance
- 📁 **Logs automatically uploaded to S3**:
  - `/app/logs/app.log`
  - `/system/cloud-init.log`
- 🗑️ **S3 Lifecycle Rule**: Logs are auto-deleted after 7 days
## 📦 Prerequisites

Before deployment, ensure:

1. Go to your GitHub repo → **Settings** → **Secrets and Variables** → **Actions**
2. Add these secrets:
   - `AWS_ACCESS_KEY_ID`
   - `AWS_SECRET_ACCESS_KEY`
   - `INSTANCE_KEY` #for this the value is all the content of your key pair.
## 🚀 How to Deploy
 
