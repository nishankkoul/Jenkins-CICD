# Jenkins End-to-End CI/CD Project using ArgoCD

In this project, we set up an end-to-end CI/CD pipeline for a Java-based application using Jenkins, ArgoCD, and various other tools and technologies like Maven, SonarQube, Docker, and Kubernetes.

## Prerequisites

Before you begin, ensure you have the following:
- Java application code hosted on a Git repository
- Jenkins server
- Kubernetes cluster
- AWS Account
- ArgoCD

## Project Workflow

1. **Setting Up the Git Repository**
   - Host the source code for the Java application on GitHub.
   - Use webhooks to trigger Jenkins pipeline on commits or pull requests.

2. **Building with Maven**
   - Build the source code using Maven.
   - Conduct unit tests and static code analysis.

3. **Code Quality Check with SonarQube**
   - Check for security vulnerabilities using SonarQube.
   - Send failure reports via email or Slack if the threshold is exceeded.

4. **Building and Uploading Docker Image**
   - Build the Docker image and upload it to DockerHub.
   - Perform these stages using a Docker agent.

5. **Continuous Delivery with ArgoCD**
   - Use Shell scripts to update Git Application Manifests.
   - ArgoCD will sync and manage the Kubernetes resources based on the Git repository state.

## Application Testing using AWS EC2

1. **Launch an AWS EC2 Instance**
   - Use the t2.micro instance type and connect via SSH.

2. **Clone the Application Repository**
   ```bash
   git clone https://github.com/nishankkoul/Jenkins-CICD.git

Follow the entire workflow of the application along with the commands here: https://nishankkoul.hashnode.dev/jenkins-end-to-end-cicd-project-using-argocd
