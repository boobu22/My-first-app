# Use official Ubuntu 22.04 Jammy base image
FROM ubuntu:22.04

# Disable interactive frontend during build
ENV DEBIAN_FRONTEND=noninteractive

# Minimal update, no extra packages installed
RUN apt-get update && apt-get upgrade -y && apt-get clean && rm -rf /var/lib/apt/lists/*

# Set default shell to bash
SHELL ["/bin/bash", "-c"]

# Set working directory
WORKDIR /workspace

# Set a non-root user if needed, otherwise root is default
# RUN useradd -ms /bin/bash devuser
# USER devuser

CMD [ "bash" ]
