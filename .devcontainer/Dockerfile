# Use Ubuntu 22.04 (Jammy) as a base
FROM ubuntu:22.04

# Avoid interactive prompts
ENV DEBIAN_FRONTEND=noninteractive

# Install OpenWrt build dependencies
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
      build-essential \
      ccache \
      git \
      subversion \
      libncurses5-dev \
      zlib1g-dev \
      gawk \
      flex \
      quilt \
      gettext \
      libssl-dev \
      python3 \
      python3-distutils \
      python3-pip \
      rsync \
      unzip \
      wget \
      file \
      binutils \
      bzip2 \
      ca-certificates \
      curl \
      libelf-dev && \
    rm -rf /var/lib/apt/lists/*

# Set the working directory inside the container
WORKDIR /workspace
