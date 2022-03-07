FROM mcr.microsoft.com/vscode/devcontainers/javascript-node:0-14-bullseye

# packages
RUN apt-get update \
    && apt-get install --no-install-recommends -y \
    vim \
    tmux

# dive
WORKDIR /install/dive
RUN wget https://github.com/wagoodman/dive/releases/download/v0.9.2/dive_0.9.2_linux_amd64.deb
RUN apt-get install -y ./dive_0.9.2_linux_amd64.deb

# shell
RUN echo "bindkey -v" >> /home/node/.zshrc
