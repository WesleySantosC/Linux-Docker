FROM ubuntu:24.04

RUN apt update && apt install -y \
    nano \
    vim \
    curl \
    wget \
    git \
    python3 \
    python3-pip \
    jq \
    tree \
    htop \
    iotop \
    sysstat \
    dnsutils \
    traceroute \
    tcpdump \
    netcat-openbsd \
    openssh-client \
    iproute2 \
    net-tools \
    procps \
    lsof \
    ncdu \
    sudo

RUN useradd -m aluno && \
    echo "aluno:linux123" | chpasswd && \
    usermod -aG sudo aluno

USER aluno
WORKDIR /home/aluno

CMD ["/bin/bash"]
