# Test Repo

A repository for testing Git workflows and Kubernetes deployments.

## Overview

This repository contains Kubernetes manifest files used for testing Git-based deployment workflows with Harness CI/CD.

## Project Structure

```
.
├── README.md
└── vivek-manifest/
    ├── deployment.yaml    # Kubernetes Deployment manifest
    └── values.yaml        # Configuration values for deployments
```

## Kubernetes Manifests

The `vivek-manifest/` directory contains:

- **deployment.yaml**: Defines the Kubernetes Deployment resource including container specs, replicas, and resource limits
- **values.yaml**: Contains configurable values that can be templated into the deployment

## Usage

### Deploy to Kubernetes

```bash
kubectl apply -f vivek-manifest/deployment.yaml
```

### With Harness

This repo can be used as a manifest source in Harness CD pipelines:
1. Connect this repo via a GitHub connector
2. Reference the manifests in your Harness Service definition
3. Deploy using a Harness CD pipeline

## Git Workflow Testing

This repository is designed for testing various Git operations:
- Branch creation and merging
- Pull request workflows
- Webhook triggers for CI/CD pipelines

## Author

**Vivek Dixit** - [@senjucanon2](https://github.com/senjucanon2)

## License

This project is for testing purposes.
