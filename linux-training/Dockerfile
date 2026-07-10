FROM ubuntu:24.04

RUN apt update && apt install -y \
    nano \
    vim \
    curl \
    wget \
    iputils-ping \
    net-tools \
    procps \
    htop \
    tree \
    sudo

RUN useradd -m aluno && \
    echo "aluno:linux123" | chpasswd && \
    usermod -aG sudo aluno

USER aluno
WORKDIR /home/aluno

CMD ["/bin/bash"]