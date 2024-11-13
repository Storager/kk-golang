FROM ubuntu:20.04
ARG GO_VERSION=1.17.13
RUN apt update \
    && apt install sudo curl wget vim git -y \
    && wget -qO- https://go.dev/dl/go${GO_VERSION}.linux-arm64.tar.gz | tar xvz -C /usr/local \
    && useradd vscode -s /bin/bash -m \
    && echo "vscode ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/vscode
USER vscode
ENV PATH=$PATH:/usr/local/go/bin:/home/vscode/go/bin