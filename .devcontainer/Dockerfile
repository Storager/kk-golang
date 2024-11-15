FROM ubuntu:20.04
RUN apt update \
    && apt install sudo curl wget vim git -y \
    && useradd vscode -s /bin/bash -m \
    && echo "vscode ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/vscode
USER vscode
ENV PATH=$PATH:/usr/local/go/bin:/home/vscode/go/bin