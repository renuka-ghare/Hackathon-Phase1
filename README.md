# Online Shop 🛍️ for Hackathon Phase 1
[![Stars](https://img.shields.io/github/stars/iemafzalhassan/online_shop)](https://github.com/iemafzalhassan/online_shop)
![Forks](https://img.shields.io/github/forks/iemafzalhassan/online_shop)
![GitHub last commit](https://img.shields.io/github/last-commit/iemafzalhassan/easyshop?color=red)
[![GitHub Profile](https://img.shields.io/badge/GitHub-iemafzalhassan-blue?logo=github&style=flat)](https://github.com/iemafzalhassan)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
<p align="center">

Welcome to the **Online Shop** project – our hackathon entry for Phase 1! This repository contains a fully functional e-commerce application built to demonstrate foundational DevOps skills in three key areas:
- **Git & GitHub**
- **Linux**
- **Docker**

## Project Overview

This repository contains my submission for Phase 1 of the Online Shop Hackathon. The primary goal was to containerize the application using Docker, resolve build issues related to missing crypto libraries, and ensure seamless deployment. This project demonstrates my competence in Git, GitHub, Linux, and Docker.

---
## Key Goals Achieved

-   Containerized the online shop application using Docker.
-   Addressed compatibility issues and resolved errors during the Docker image build.
-   Documented all steps and considerations in the README.

---

## 1.  **Dockerization**

    *   Created a `Dockerfile` tailored for the application, ensuring all dependencies were included.
    *   Leveraged multi-stage builds to reduce the size of the final image.
    *   Verified successful deployment of the application within a Docker container.

    Commands used:
        -   `docker build -t online_shop_app .`
        -   `docker run -d -p 80:80 online_shop_app`

## 2.  **Addressing the Crypto Error**

    *   Identified the `crypto`-related error during `npm run build` within the container.
    *   Implemented the solution by updating the Node version to a more recent version that includes the `crypto` libraries.
    *   Justification for implementation: Simplest method with less code changes. The other methods might require code modification or other more complex configurations.

## 3.  **Nginx Integration (as Reverse Proxy)**

    *   Setup reverse proxy
---

## Challenges Faced

-   Difficulty in the configuration with libraries related to crypto
-   Setting up reverse proxy can be a bit overwhelming since there is so much to configure.

## Lessons Learned

-   Debugging Docker build issues often requires a deep understanding of Node.js package dependencies.
-   Efficient Dockerization is crucial for maintaining application performance.
-   Importance on using reverse proxy instead of serving content directly.
---

## Branch Information

This submission is located in the `Renuka_Dockerfile_For_Hackathon` branch.

### Git & GitHub

- **Repository Management:** Fork and clone the repository, then create a new branch for your work. Ensure your commit history is clean and well-documented.
- **Collaboration Practices:** Follow best practices for version control by making descriptive commits, creating pull requests, and engaging in code reviews.
- **Workflow Optimization:** Identify any areas where the Git workflow can be improved and document your suggestions for future enhancements.

### Linux

- **Command Line Proficiency:** Review the code for examples of Linux command usage. Test and verify that file operations, system scripts, and environment configurations are functioning as expected.
- **System Administration:** Examine how the application handles Linux-based operations such as permissions, file management, and process monitoring. If you see room for improvement, implement those changes and document them.
- **Documentation:** Clearly document any Linux-related enhancements you make, explaining how they optimize the project’s performance or usability.

### Docker

- **Containerization Principles:** Even though a Dockerfile is not provided in this repository, consider how you would package and deploy this application using Docker. Reflect on the design decisions that would facilitate containerization.
- **Conceptual Improvements:** Propose any modifications or improvements that could make future Docker integration smoother. Document your suggestions clearly in your pull request.
- **Code Readiness:** Ensure the codebase is structured in a way that aligns with Docker best practices, preparing it for eventual containerized deployment on AWS EC2 / Azure VM / Google Compute Engine (Your Choice of Cloud).

---
Happy Learning :)
