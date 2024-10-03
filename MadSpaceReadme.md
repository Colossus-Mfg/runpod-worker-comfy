# MadSpace Docker Image Builder

This README provides instructions on how to build and deploy Docker images for various workflows in the MadSpace project.

## Prerequisites

- Docker installed on your system
- Access to the required Docker files (e.g., Dockerfile.workflow1)
- Hugging Face access token (if required)

## Building the Docker Image

Use the following command template to build the Docker image for workflow 1:

```bash
docker build -f Dockerfile.workflow1 -t <dockerhub_username>/runpod-worker-madespace:<tag> --build-arg HUGGINGFACE_ACCESS_TOKEN=<your_huggingface_access_token> --platform linux/amd64 ./
```

Replace `<dockerhub_username>` with your Docker Hub username, `<tag>` with the desired tag for your image, and `<your_huggingface_access_token>` with your actual Hugging Face access token.

## Workflow 1: Basic Workflow

### Dockerfile

The Dockerfile for this workflow is located in the `Dockerfile.workflow1` file.
