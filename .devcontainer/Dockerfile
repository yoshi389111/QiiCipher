# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.177.0/containers/alpine/.devcontainer/base.Dockerfile

# [Choice] Alpine version: 3.13, 3.12, 3.11, 3.10
ARG VARIANT="3.13"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-alpine-${VARIANT}

RUN apk add --no-cache \
        shellcheck \
        shfmt \
        openssl

USER vscode

RUN sh -c 'wget -O- https://git.io/shellspec | sh -s -- --yes'
