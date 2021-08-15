# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.191.0/containers/ubuntu/.devcontainer/base.Dockerfile

# [Choice] Ubuntu version: bionic, focal
ARG VARIANT="focal"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-${VARIANT}

# Give permissions to repo folder
RUN mkdir /home/vscode/repo
RUN chmod 777 /home/vscode/repo
USER vscode

RUN sudo apt-get update

# Install python
RUN sudo apt-get install python3 -y
RUN sudo ln -s /usr/bin/python3 /usr/bin/python & \
    sudo ln -s /usr/bin/pip3 /usr/bin/pip

