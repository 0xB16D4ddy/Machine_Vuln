# kali/Dockerfile
FROM kalilinux/kali-rolling

# Install tools commonly used in penetration testing
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    metasploit-framework \
    nmap \
    john \
    hydra \
    git \
    python3 \
    netcat-traditional \ 
    net-tools

# Set alias to use 'nc' as a command
RUN update-alternatives --install /usr/bin/nc nc /bin/nc.traditional 10

CMD ["/bin/bash"]
