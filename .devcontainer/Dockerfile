FROM ubuntu:22.04

RUN apt-get update && \
    apt-get install -y sudo && \
    useradd -m ubuntu && \
    echo "ubuntu ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

# Optionally, set root password (empty for now)
RUN echo "root::0:0:root:/root:/bin/bash" | chpasswd

USER ubuntu
WORKDIR /home/ubuntu
