FROM mcr.microsoft.com/devcontainers/java:0-17



RUN export DEBIAN_FRONTEND=noninteractive && apt update && \
    apt upgrade -y && \
    apt install -y python3-pip &&\
    pip install awscli awscli-local && pip cache purge &&\
    apt clean -y && rm -rf /var/lib/apt/lists/* 

USER root