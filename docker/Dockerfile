FROM ubuntu:18.04

LABEL "title"="SEEK-AI Text-Summarization" \
      "description"="SEEK-AI Text-Summarization application" \
      "version"="1.0.0"

# Install basic software
RUN apt-get update && \
    apt-get install -y \
      build-essential \
      gcc \
      g++ \
      git \
      python3-dev \
      python3-pip \
      vim

RUN pip3 install \
    gensim \
    wget \
    nltk \
    tensorflow

# Set up environs
ENV LANG=C.UTF-8
ENV PYTHONIOENCODING=utf-8
ENV PYTHONDONTWRITEBYTECODE=1

WORKDIR /seek-ai/txt-sum
ENTRYPOINT while true; do echo "Text Summarization"; sleep 5; done
