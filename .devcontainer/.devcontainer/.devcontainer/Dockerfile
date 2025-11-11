# Start from an official base image
FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Install Terraform and AWS CLI
RUN apt-get update && apt-get install -y unzip curl awscli && \
    curl -fsSL https://releases.hashicorp.com/terraform/1.9.5/terraform_1.9.5_linux_amd64.zip -o terraform.zip && \
    unzip terraform.zip && \
    mv terraform /usr/local/bin/ && \
    rm terraform.zip && \
    terraform -version
