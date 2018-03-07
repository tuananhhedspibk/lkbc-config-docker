FROM ubuntu:16.04

RUN apt-get update \
    && apt-get install -y \
    build-essential \
    ca-certificates \
    gcc \
    git \
    libpq-dev \
    make \
    python-pip \
    python2.7 \
    python2.7-dev \
    ssh \
    && apt-get autoremove \
    && apt-get clean

RUN pip install --upgrade pip
RUN pip install numpy
RUN pip install matplotlib
RUN pip install pyvi
RUN pip install gensim
RUN apt-get --assume-yes install python-tk
