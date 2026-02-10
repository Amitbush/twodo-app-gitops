# 🎡 Twodo - GitOps & CD Control

The Source of Truth for the application's deployment state.

## ⚙️ How it Works
This repository utilizes **ArgoCD** to implement a GitOps workflow. It contains the **Root Application** definition which monitors the App Repository and ensures the EKS cluster matches the desired state defined in Git.

## 📂 Project Structure
- `apps/` - Contains ArgoCD Application manifests (e.g., `twodo-application.yaml`).

## 🎯 Key Features
- **Self-Healing**: Automatic reversion of manual cluster changes to match Git.
- **Drift Detection**: Real-time monitoring of configuration differences.
- **Centralized Control**: Full visibility into deployment versions and history via the ArgoCD Dashboard.

---
Managed by Terraform & ArgoCD.