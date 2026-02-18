# 🚀 GitHub Pages Deployment with GitHub Actions

> **Project 1: CloudOps Academy End of Cohort 1 Portfolio**

![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-222222?style=for-the-badge&logo=githubpages&logoColor=white)
![CI/CD](https://img.shields.io/badge/CI/CD-Automation-brightgreen?style=for-the-badge)

## 🎯 What This Project Demonstrates

This project implements a **continuous integration and continuous deployment (CI/CD) pipeline** using GitHub Actions to automatically deploy a static website to GitHub Pages. Key learning objectives include:

| Concept | Why It Matters |
|---------|---------------|
| **GitHub Actions Workflows** | Automate repetitive tasks using event-driven YAML configuration |
| **Path-Based Triggers** | Optimize pipeline efficiency by running jobs only when relevant files change |
| **GitHub Pages Integration** | Deploy static sites directly from a repository without manual intervention |
| **Least-Privilege Permissions** | Secure automation by granting tokens only the permissions they need |
| **Infrastructure as Code (IaC)** | Define deployment logic in version-controlled files for reproducibility |

> 💡 **Core Takeaway**: A single push to `main` that modifies `index.html` triggers an automated, verified deployment—demonstrating how DevOps practices reduce manual error and accelerate feedback loops.

## ⚙️ How to Trigger the Deployment

The workflow is configured to run **automatically** under these conditions:

```yaml
on:
  push:
    branches: [main]
    paths: ['index.html']  # ← Only triggers when this file changes