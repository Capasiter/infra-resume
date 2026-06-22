# 🚀 Automated Infrastructure Resume Pipeline

Welcome to my infrastructure-as-code resume repository. This project demonstrates a production-grade CI/CD pipeline that automatically builds, formats, and deploys my professional engineering resume.

## 🛠️ The DevOps Pipeline Architecture
Every time a code modification is pushed to this repository, a continuous integration workflow triggers automatically:
1. **Source Control:** Code revisions are managed natively inside a Linux (WSL2) local environment and pushed to GitHub.
2. **CI/CD Automation:** GitHub Actions spins up an isolated `ubuntu-latest` virtual runner on every commit.
3. **Compilation:** A automated Marp compiler step processes the raw Markdown (`resume.md`), standardizes the styling matrix, and outputs a clean, production-ready PDF.
4. **Artifact Deployment:** The verified PDF is compiled and uploaded as a downloadable deployment artifact.

## 🖥️ Target Homelab Environment
The core systems engineering competencies highlighted in this resume are actively developed and maintained within a dedicated bare-metal testing environment:
* **Hypervisor:** Proxmox VE managing clustered microservices, nested virtualization sandboxes, and Unraid storage arrays.
* **Configuration Management:** Ansible playbooks for automated bare-metal OS provisioning and declarative package state mapping.
* **Containerization:** Redundant application workloads orchestrated via Docker and Portainer, utilizing Nginx reverse proxies for layer-7 load balancing and high-availability routing.
