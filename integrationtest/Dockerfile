FROM ubuntu:latest
RUN apt-get update && apt-get install -y \
    wget \
    && rm -rf /var/lib/apt/lists/* \
    && wget https://github.com/Yelp/dumb-init/releases/download/v1.2.0/dumb-init_1.2.0_amd64 -q -O /usr/local/bin/dumb-init \
    && wget https://storage.googleapis.com/kubernetes-release/release/v1.13.2/bin/linux/amd64/kubectl -q -O /usr/local/bin/kubectl \
    && chmod a+x /usr/local/bin/kubectl /usr/local/bin/dumb-init
CMD ["bash"]
