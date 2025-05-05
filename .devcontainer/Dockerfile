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

# Let's add a fancy prompt!
RUN echo "PS1='🐳 \[\033[1;36m\]\h \[\033[1;34m\]\W\[\033[0;35m\] \[\033[1;36m\]# \[\033[0m\]'" > ~/.bashrc
