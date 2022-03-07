FROM mcr.microsoft.com/vscode/devcontainers/javascript-node:0-14-bullseye

# packages
RUN apt-get update \
    && apt-get install --no-install-recommends -y \
    vim \
    tmux

# shell
RUN echo "bindkey -v" >> /home/node/.zshrc
