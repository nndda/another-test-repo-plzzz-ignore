FROM debian:12-slim

WORKDIR /site

# COPY \
#   ../../package.json \
#   ../../bun.lock \
#   requirements.txt \
#   ./

RUN apt update && \
    apt install -y --no-install-recommends \
    curl \
    git \
    ca-certificates \
    python3 \
    unzip \
    && rm -rf /var/lib/apt/lists/* \
    && ln -s /usr/bin/python3 /usr/bin/python

# Bun
RUN curl -fsSL https://bun.com/install | bash -s "bun-v1.3.14"
