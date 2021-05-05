FROM nvidia/cuda:11.3.0-cudnn8-devel-ubuntu20.04

ENV SHELL /bin/bash
ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update && \
    apt-get install -y python3.8 python3.8-venv python3-pip &&\
    apt-get install -y graphviz git curl && \
    apt-get autoremove -y &&\
    apt-get clean &&\
    rm -rf /usr/local/src/*

CMD ['bin/bash']
