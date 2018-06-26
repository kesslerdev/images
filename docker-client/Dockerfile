FROM ubuntu:18.04

# installing deps curl
RUN apt-get update \
    && apt-get install -y curl \
    && apt-get -y autoremove \
    && apt-get autoremove -y \
    && apt-get autoclean -y \
    && apt-get clean -y \
    && rm -rf \
    /tmp/* \
    /usr/share/doc \
    /usr/share/man \
    /usr/share/doc

# docker
RUN curl -L -s https://download.docker.com/linux/static/stable/x86_64/docker-17.12.0-ce.tgz | \
    tar zxv docker/docker \
    && mv docker/docker /bin/docker