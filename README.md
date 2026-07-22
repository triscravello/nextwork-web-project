# Java Web App Deployment with AWS CI/CD

Welcome to this project combining Java web application development with AWS DevOps and CI/CD services!

<br>

## Table of Contents
- [Introduction](#introduction)
- [Technologies](#technologies)
- [Setup](#setup)
- [Contact](#contact)
- [Conclusion](#conclusion)

<br>

## Introduction

This project is my introduction to building and deploying a Java web application using AWS while learning modern DevOps practices.

The deployment pipeline I'm building around this application is invisible to end users, but it automates software delivery, making deployments faster, more reliable, and easier to maintain.

### Why I'm Building This Project

- I'm developing hands-on AWS DevOps skills to complement my full-stack software engineering experience and prepare for cloud-focused engineering roles.
- This project is part of a larger CI/CD learning journey where I'm building production-inspired deployment pipelines using AWS services from source control through automated deployment.

<br>

## Technologies

Here's what I'm using throughout this project:

- **Amazon EC2** – Developing and hosting my application on a cloud-based Linux server.
- **Visual Studio Code** – Connected remotely to my EC2 instance using Remote SSH for cloud-based development.
- **Git & GitHub** – Version control and source code management for tracking every change to the application.
- **[COMING SOON] AWS CodeArtifact** – Private package management for storing project dependencies.
- **[COMING SOON] AWS CodeBuild** – Automated builds, testing, and artifact creation.
- **[COMING SOON] AWS CodeDeploy** – Automated deployments to EC2 instances.
- **[COMING SOON] AWS CodePipeline** – End-to-end CI/CD pipeline connecting GitHub, build, test, and deployment stages.

### Challenges & Solutions

- **Challenge:** Connecting VS Code to my EC2 instance through Remote SSH.
  - **Solution:** Verified my SSH key permissions, EC2 security group rules, and connection settings before successfully establishing the remote connection.

- **Challenge:** GitHub rejected my password during `git push`.
  - **Solution:** Generated a GitHub Personal Access Token (PAT) and used it instead of my account password for secure authentication.

<br>

## Setup

To run this project locally:

1. Clone the repository

```bash
git clone https://github.com/triscravello/nextwork-web-project.git
```

2. Enter the project directory

```bash
cd nextwork-web-project
```

3. Install dependencies

```bash
mvn install
```

### Troubleshooting

- If `git push` fails with an authentication error, make sure you're using a **GitHub Personal Access Token** instead of your GitHub password.
- If VS Code cannot connect to EC2, verify:
  - Your EC2 instance is running.
  - Port 22 is open in the security group.
  - Your SSH key has the correct permissions (`chmod 400`).
  - You're using the correct username (`ec2-user`) and private key.

<br>

## Contact

**Tristan Cravello**

💼 LinkedIn: https://www.linkedin.com/in/tristan-cravello-3b6500146/

🌐 Portfolio: https://triscravello.github.io/tristan-portfolio-site/

📧 Email: tlcravello@gmail.com

<br>

## Conclusion

Thank you for exploring this project!

This is the first step in a larger AWS DevOps journey where I'll continue building a complete CI/CD pipeline using AWS services. Each project builds on the previous one, gradually moving toward production-ready cloud deployments and modern software delivery practices.

Special thanks to **NextWork** for creating an excellent hands-on learning experience that makes cloud computing and DevOps approachable.

➡️ Check out the NextWork project series:
https://learn.nextwork.org/projects/aws-devops-vscode?track=high

