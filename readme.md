
# 📘 SOP: Git Branching Strategy

## 📌 Overview
This document defines the **Standard Operating Procedure (SOP)** for the Git branching strategy used in this project.  
It ensures **code quality**, **controlled releases**, and **smooth collaboration** across teams.

---

## 🎯 Purpose
- Maintain a **clean and stable codebase**
- Enable **parallel development**
- Reduce merge conflicts
- Support **safe and predictable deployments**

---

## 📂 Scope
This SOP applies to:
- All Git repositories
- Developers, reviewers, and DevOps engineers
- Development, staging, and production environments

---

## 🌿 Branch Types

### 🔐 `main` (Production Branch)
- Contains **production-ready code**
- Always stable and deployable
- ❌ No direct commits allowed
- ✔ Changes only via approved merge requests

---

### 🧪 `develop` (Integration Branch)
- Contains latest **integrated features**
- Used for testing and validation
- Created from `main`
- Merges only from `feature/*` branches

---

### ✨ `feature/*` (Feature Branches)
- Used for **new features or enhancements**
- Created from `develop`
- Naming convention:
  ```bash
  feature/<feature-name>
