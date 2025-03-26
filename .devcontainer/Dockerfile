FROM mcr.microsoft.com/devcontainers/cpp:1-debian-12

COPY debian.sources /etc/apt/sources.list.d/debian.sources

RUN sudo apt-get update
RUN sudo apt-get upgrade -y

# install dependency
RUN sudo apt-get install -y git g++ cmake ninja-build libssl-dev

# install clangd
RUN sudo apt-get install -y clangd-19
RUN sudo update-alternatives --install /usr/bin/clangd clangd /usr/bin/clangd-19 100