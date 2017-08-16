FROM ubuntu:16.04

RUN apt-get update -q; apt-get install -y wget bzip2 git
RUN wget https://repo.continuum.io/miniconda/Miniconda2-latest-Linux-x86_64.sh; \
    bash Miniconda2-latest-Linux-x86_64.sh -b -p /conda
ENV PATH /conda/bin:$PATH

RUN conda install anaconda-client conda-build; \
    conda update --all

