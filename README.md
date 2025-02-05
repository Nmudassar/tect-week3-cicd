# # CI/CD and SDLC Research

## 1. What is Continuous Integration (CI)?

Continuous Integration (CI) is the practice of frequently merging code changes into a shared repository, followed by automated testing.

### Benefits of CI:

- Detects and fixes integration issues early.
- Reduces debugging time.
- Ensures stable builds.
- Enhances code quality with automated testing.
- Improves team collaboration.

## 2. What is Continuous Delivery (CD)?

Continuous Delivery (CD) automates the process of preparing code changes for production release by running tests and packaging applications.

### Benefits of CD:

- Faster and safer releases.
- Reduces manual deployment risks.
- Ensures reliable software delivery.
- Minimizes downtime during updates.

## 3. Difference Between Continuous Delivery (CD) and Continuous Deployment (CDE)

| Feature    | Continuous Delivery (CD)                    | Continuous Deployment (CDE)                      |
| ---------- | ------------------------------------------- | ------------------------------------------------ |
| Deployment | Requires manual approval before deployment  | Fully automated deployment                       |
| Control    | More control over what goes into production | Less control, every successful build is deployed |
| Use Case   | Suitable for compliance-heavy industries    | Suitable for fast-paced development environments |

## 4. What is Jenkins?

Jenkins is an open-source automation server that facilitates CI/CD by automating software builds, testing, and deployment.

### Why Use Jenkins?

- Automates repetitive CI/CD tasks.
- Provides a plugin-rich ecosystem.
- Integrates with various tools (Git, Docker, Kubernetes, etc.).
- Supports distributed builds for scalability.

### Benefits of Jenkins:

- Open-source and widely used.
- Highly customizable with plugins.
- Scalable and supports parallel builds.

### Disadvantages of Jenkins:

- Requires maintenance and frequent updates.
- Complex configurations for large-scale implementations.
- Performance issues when dealing with too many plugins.

## 5. Stages of Jenkins

1. **Commit Stage** - Code is committed to a repository.
2. **Build Stage** - Jenkins pulls the code and builds it.
3. **Test Stage** - Automated tests run to validate the build.
4. **Deploy Stage** - The verified build is deployed to an environment.
5. **Monitoring & Feedback** - Logs and performance metrics are collected.

## 6. Alternatives to Jenkins

- **GitHub Actions** - Natively integrated with GitHub.
- **GitLab CI/CD** - Built-in CI/CD for GitLab repositories.
- **CircleCI** - Cloud-based CI/CD with fast builds.
- **Travis CI** - Simple CI/CD for open-source projects.
- **Azure DevOps** - Microsoft’s CI/CD service.
- **ArgoCD** - Kubernetes-native continuous deployment tool.

## 7. Why Build a CI/CD Pipeline? Business Value

- Reduces time-to-market.
- Enhances software reliability and quality.
- Minimizes human errors in deployment.
- Supports agile development practices.
- Enables quick feedback loops.

## 8. CI/CD Pipeline Diagram

(Refer to the attached diagram for a general CI/CD workflow.)

## 9. Understanding the SDLC Workflow

The Software Development Life Cycle (SDLC) consists of the following phases:

1. **Plan** – Define project scope and requirements.
2. **Design** – Create architecture, wireframes, and database structures.
3. **Develop** – Write and integrate code based on design specifications.
4. **Test** – Validate code functionality and performance.
5. **Deploy** – Deploy the software to production.
6. **Maintain** – Monitor and update the application.

## 10. References

- Jenkins Documentation: https://www.jenkins.io/
- CI/CD Best Practices: https://martinfowler.com/articles/continuous-integration.html
- SDLC Overview: https://www.ibm.com/cloud/learn/sdlc
