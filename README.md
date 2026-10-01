# DevOps Infrastructure Workspace: Docker Fundamentals to Advanced Architectures

A hands-on engineering sandbox dedicated to mastering containerisation, microservices management, and infrastructure optimization. This repository documents my practical transition from standard local development to industry-grade DevOps environments, focusing on building high-performance, secure, and production-ready containerised applications.

## 🚀 Core Objectives & Technical Implementations

* **Single-Stage Containerisation:** Designing standard Dockerfiles for application packaging, focusing on environmental isolation, core commands (`FROM`, `RUN`, `COPY`, `CMD`), and proper layer caching strategies.
* **Multi-Stage Build Optimization:** Engineering advanced multi-stage Dockerfiles to drastically reduce production image footprints (using minimal base images like `python-slim` and `alpine`), slicing build bloat while enhancing container security.
* **Network & Port Routing Architecture:** Implementing absolute host-to-container port mapping schemas (`-p`), handling dynamic environment variables (`ENV`), and configuring zero-trust network parameters locally before cloud deployment.
* **Persistent Storage Architecture:** Executing Docker Volumes and Bind Mount operations to maintain stateful local data consistency across continuous container lifecycles.

## 🛠️ Tech Stack & Tools Mastered
* **Container Core:** Docker, Docker Desktop for macOS (Apple Silicon integration)
* **Base Environments:** Alpine Linux, Ubuntu core distributions
* **Application Services:** Python (Flask/WSGI microservices), Nginx (High-performance web proxying)
* **Version Control:** Git architecture (Time-travel version debugging, branches, origin tracking)

---
*Aligning system architecture with enterprise performance standards.*
