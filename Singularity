Bootstrap: docker
From: debian:latest

%post
    apt-get update && apt-get -y install locales
    locale-gen en_US.UTF-8
    apt-get -y install automake autoconf pkg-config libcurl4-openssl-dev libjansson-dev libssl-dev libgmp-dev zlib1g-dev
    cd /usr/ports/ftp/curl; make install
    apt-get clean
    git clone https://github.com/fireworm71/veriumMiner.git
    cd veriumMiner
