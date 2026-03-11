# devsecops-security-pipeline
**# DevSecOps Automated Security Pipeline

This project demonstrates a secure CI/CD pipeline integrating security testing tools.

## Tools Used
- Jenkins
- SonarQube
- OWASP ZAP
- TruffleHog
- Docker

## Features
- Secret detection in source code
- Static Application Security Testing (SAST)
- Dynamic Application Security Testing (DAST)
- Automated vulnerability scanning in CI/CD

## Workflow
Developer → GitHub → Jenkins Pipeline → Security Scans → Deployment

## Security Scans
- TruffleHog scans commits for exposed secrets
- SonarQube performs static code analysis
- OWASP ZAP performs dynamic vulnerability scanning

## Conclusion
This project demonstrates DevSecOps practices by integrating security into the software development lifecycle.**
