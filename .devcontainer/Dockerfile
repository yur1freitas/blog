FROM debian:13.2-slim

ENV LANG=pt_BR.UTF-8
ENV LANGUAGE=pt_BR.UTF-8
ENV LC_ALL=pt_BR.UTF-8

ENV BUN_INSTALL=/root/.bun
ENV PATH="$BUN_INSTALL/bin:$PATH"

RUN apt update && \
    apt install -y git fish vim curl unzip locales locales-all && \
    rm -rf /var/lib/apt/lists/* && \
    git config --global editor.core vim

RUN curl -fsSL https://bun.com/install | bash

