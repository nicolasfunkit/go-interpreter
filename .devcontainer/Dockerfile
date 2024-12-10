# Update the NODE_VERSION arg in docker-compose.yml to pick a Node version: 18, 16, 14
ARG NODE_VERSION=16
FROM mcr.microsoft.com/devcontainers/javascript-node:${NODE_VERSION}

# VARIANT can be either 'hugo' for the standard version or 'hugo_extended' for the extended version.
ARG VARIANT=hugo_extended
# VERSION can be either 'latest' or a specific version number
ARG VERSION=latest

# Download Hugo
RUN apt-get update && apt-get install -y ca-certificates openssl git curl lftp && \
    rm -rf /var/lib/apt/lists/*

# [Optional] Uncomment this section to install additional OS packages you may want.
#
#RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
#     && go install github.com/go-task/task/v3/cmd/task@latest
#RUN sudo -u node go install github.com/go-task/task/v3/cmd/task@latest
# [Optional] Uncomment if you want to install more global node packages
# RUN sudo -u node npm install -g <your-package-list-here>

