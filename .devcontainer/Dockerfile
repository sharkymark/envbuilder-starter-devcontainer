FROM ubuntu

USER root

RUN DEBIAN_FRONTEND="noninteractive" apt-get update -y && \
    apt-get install -y \
    vim \
    sudo \
    curl \
    jq \
    figlet \
    wget

RUN useradd -m -s /bin/bash -G sudo coder
USER coder
