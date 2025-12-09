FROM ubuntu:22.04

RUN apt-get update && \
    DEBIAN_FRONTEND=noninteractive apt-get install -y \
        make \
        texlive-latex-base \
        texlive-latex-recommended \
        texlive-latex-extra \
        texlive-fonts-recommended \
        texlive-fonts-extra \
        latexmk \
        poppler-utils \
        imagemagick \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /work
