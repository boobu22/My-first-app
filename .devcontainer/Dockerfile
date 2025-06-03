FROM ubuntu:22.04

# Just update apt cache, no extra packages installed
RUN apt-get update && rm -rf /var/lib/apt/lists/*

# Create user 'ubuntu' (without sudo)
RUN useradd -m ubuntu

USER ubuntu
WORKDIR /home/ubuntu
