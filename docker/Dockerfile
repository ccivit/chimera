FROM nvidia/cuda:9.0-cudnn7-runtime-ubuntu16.04

RUN apt-get update && apt-get install -y \
	wget \
	vim \
	bzip2 \ 
	nano \ 
	python3 \ 
	python-pip3

RUN pip3 install --upgrade pip

WORKDIR /data_project

RUN pip3 install requirements.txt

ENTRYPOINT ["/bin/bash"]
