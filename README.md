This is a multiarch Docker image for deployment tasks. The aim is to focus on Docker tools that will be needed to deploy on Kubernetes. Everything else should probably go to Dockerfile (use multistage builds if needed) or other images should be created.

The main reason for this image was to have all tools which Terraform might need (AWS IAM authenticator). Then to have a helm image with all the useful plugins... And so on and on.

[Docker Hub](https://hub.docker.com/repository/docker/ernestas/deploy)
[Github Container Registry](https://github.com/ernetas/deploy/pkgs/container/deploy)

Includes:
- Terraform
- Terragrunt
- AWS IAM authenticator
- AWS CLI v2
- Azure CLI
- kubectl
- helm with a couple of plugins
- helmfile
- velero
