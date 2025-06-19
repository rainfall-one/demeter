# syntax=docker/dockerfile:1
FROM mcr.microsoft.com/devcontainers/typescript-node:dev-22-bookworm

# [Optional] Install any additional OS packages or tools here
RUN apt-get update \
    && rm -rf /var/lib/apt/lists/*

# Set up default user (devcontainers will override if needed)
