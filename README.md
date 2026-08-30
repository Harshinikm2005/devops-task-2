# DevOps Task 2: Jenkins CI/CD Pipeline

## Objective
Automate the build, test, and deployment process of a containerized web application using Jenkins and Docker.

---

## Tools Used
- **CI/CD Automation:** Jenkins
- **Containerization:** Docker
- **Version Control:** Git & GitHub

---

## Pipeline Architecture & Stages
1. **Checkout:** Pulls the source code and Dockerfile from the GitHub repository.
2. **Build:** Builds the Docker container image tagged with the unique Jenkins build number (`my-web-app:<BUILD_NUMBER>`).
3. **Test:** Validates the Nginx configuration syntax inside the container using `nginx -t`.
4. **Deploy:** Stops and cleans up any existing container instances and launches the updated container on port `8085`.

---

## Verification & Screenshots

### 1. Pipeline Stages (Build #3 Success)
![Pipeline Stages](jenkins-stages.png)

### 2. Jenkins Job Dashboard
![Jenkins Dashboard](jenkins-dashboard.png)

### 3. Pipeline SCM Configuration
![Jenkins Configuration](jenkins-config.png)

### 4. Deployed Web Application
![Deployed Application](deployed-app.png)

---

