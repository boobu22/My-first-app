FROM ubuntu:22.04

ENV DEBIAN_FRONTEND=noninteractive

# Create non-root user 'devuser' with sudo privileges (no password)
RUN apt-get update && apt-get install -y sudo ca-certificates curl && rm -rf /var/lib/apt/lists/* && \
    useradd -m -s /bin/bash devuser && \
    echo "devuser ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

USER devuser
WORKDIR /home/devuser

# (Optional) install Nexus prerequisites or scripts here
