📘 README.md — CI/CD with GitHub Actions → Minikube → ArgoCD
🚀 Overview

This repository implements a complete CI/CD pipeline where:

GitHub Actions

Builds the Docker image

Loads it into the Minikube Docker daemon

Updates k8s/kustomization.yaml with the new image tag

Commits the updated manifests back to the repo

ArgoCD

Watches the k8s/ folder

Auto-syncs updates into the local Minikube cluster

Allows manual sync verification through the ArgoCD UI

Minikube

Runs locally

Renders & deploys all Kubernetes manifests

Uses ArgoCD to deploy the application automatically

