FROM python:3.9
RUN apt update \
    && apt install sudo curl wget vim git -y \
    && useradd vscode -s /bin/bash -m \
    && echo "vscode ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/vscode
USER vscode
