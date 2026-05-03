# Java Web App CI CD Pipeline | Jenkins, Maven, SonarQube, Nexus

![CI/CD](https://img.shields.io/badge/CI/CD-Jenkins-red)
![Java](https://img.shields.io/badge/Java-WebApp-orange)
![Maven](https://img.shields.io/badge/Maven-Build-blue)
![SonarQube](https://img.shields.io/badge/Code%20Quality-SonarQube-yellow)
![Nexus](https://img.shields.io/badge/Artifacts-Nexus-success)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

---

## Project Overview

Built a CI CD pipeline for a Java web application using Jenkins.

The pipeline integrates GitHub, Maven, SonarQube, and Nexus to automate build, code analysis, artifact storage, and deployment.

GitHub webhooks trigger the pipeline on every code commit.

---

## Key Impact

* Automated full build and deployment pipeline
* Integrated code quality checks using SonarQube
* Managed artifacts using Nexus repository
* Reduced manual deployment effort
* Improved build consistency and reliability

---

## Architecture

```id="p7x4sd"
Developer → GitHub → Jenkins → Maven Build → SonarQube → Nexus → Tomcat on AWS EC2 → Users
```

---

## Tech Stack

* Jenkins
* GitHub
* Apache Maven
* SonarQube
* Sonatype Nexus Repository
* Apache Tomcat
* AWS EC2
* Linux
* Java

---

## CI CD Workflow

1. Developer pushes code to GitHub
2. Webhook triggers Jenkins pipeline
3. Maven builds project and creates WAR file
4. SonarQube runs code quality analysis
5. Artifact stored in Nexus repository
6. Jenkins deploys application to Tomcat on EC2

---

## Project Structure

```id="n4v8kx"
.
├── src/main/webapp/
│   ├── WEB-INF/
│   │   └── web.xml
│   └── index.jsp
├── Jenkinsfile
├── pom.xml
├── tomcat-users.xml
├── README.md
└── LICENSE
```

---

## Setup Guide

### Clone Repository

```id="g2s7qm"
git clone https://github.com/kd-abhidev/App-Deployment-Jenkins-with-Maven-SonarQube-Nexus.git
cd App-Deployment-Jenkins-with-Maven-SonarQube-Nexus
```

---

### Build Application

```id="w8f3lz"
mvn clean package
```

---

### Run Jenkins Pipeline

* Configure Jenkins with required plugins
* Add GitHub webhook
* Configure SonarQube and Nexus
* Run pipeline using Jenkinsfile

---

### Deploy to Tomcat

* Configure Tomcat on EC2
* Add user in tomcat-users.xml
* Deploy WAR file

---

## What You Learn

* CI CD pipeline design with Jenkins
* Maven build lifecycle
* Code quality analysis with SonarQube
* Artifact management using Nexus
* Web app deployment on Tomcat

---

## Challenges Solved

* Configured webhook based triggers
* Integrated multiple DevOps tools
* Managed artifact storage and deployment
* Improved pipeline reliability

---

## Future Improvements

* Add Docker based deployment
* Add Kubernetes deployment
* Add automated testing stage
* Add monitoring integration

---

## Outcome

Built an automated CI CD pipeline that handles build, code analysis, artifact storage, and deployment, improving deployment speed and reliability.

