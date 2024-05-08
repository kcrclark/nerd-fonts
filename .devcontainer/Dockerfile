ARG VARIANT=3
FROM mcr.microsoft.com/vscode/devcontainers/python:${VARIANT}

LABEL Name="FontForge" Version="2020-07-31"

RUN apt-get update \
    && export DEBIAN_FRONTEND=noninteractive \
    && apt-get install --no-install-recommends -y bc fontforge \
    && fontforge --version 2>&1

EXPOSE 8080