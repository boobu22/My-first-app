# Use official Ubuntu 22.04 base image
FROM ubuntu:22.04

# Install sudo and any other packages you want (e.g. openjdk-11-jdk)
RUN apt-get update && \
    apt-get install -y sudo openjdk-11-jdk curl vim && \
    rm -rf /var/lib/apt/lists/*

# Create ubuntu user and give passwordless sudo
RUN useradd -m ubuntu && echo "ubuntu ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

# Set ubuntu as default user
USER ubuntu
WORKDIR /home/ubuntu
