# three-tier-be

Backend microservice for the Three-Tier DevSecOps application.

## Technology Stack
- **Runtime:** Node.js 18
- **Framework:** Express.js
- **Database:** MongoDB
- **Container:** Docker (Alpine-based multi-stage build)

## CI/CD Pipeline
- **Jenkins:** Multibranch Pipeline with webhook triggers
- **Security Scanning:** SonarQube + Trivy
- **Registry:** AWS ECR with automated lifecycle policies
- **Deployment:** ArgoCD GitOps with Image Updater

## Image Tagging
Images use date-based semantic versioning: `YYYYMMDD-BUILD` (e.g., `20241120-1`)

## Local Development
```bash
npm install
npm start
```

## Environment Variables
- `MONGO_CONN_STR` - MongoDB connection string
- `MONGO_USERNAME` - MongoDB username  
- `MONGO_PASSWORD` - MongoDB password
