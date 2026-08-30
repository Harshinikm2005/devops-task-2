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
1. **Checkout:** Clones the source code and Dockerfile from the GitHub repository.
2. **Build:** Builds the Docker container image tagged with the unique Jenkins build number (`my-web-app:<BUILD_NUMBER>`).
3. **Test:** Validates the Nginx configuration syntax inside the container using `nginx -t`.
4. **Deploy:** Stops and cleans up any existing container instances and launches the updated container on port `8085`.

---

## Verification & Documentation
- **Execution Proof:** [Download / View Task 2 Screenshot PDF](Task%202%20Screenshot.pdf)
- **Live Deployment Output:** `http://localhost:8085`

