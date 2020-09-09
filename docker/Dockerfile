FROM nvidia/cuda:9.0-cudnn7-runtime-ubuntu16.04

RUN apt-get update 
RUN apt-get install -y software-properties-common \
 		       	wget \
			vim \
			bzip2 \ 
			nano
			
RUN add-apt-repository ppa:deadsnakes/ppa

RUN apt-get install
	python3.6 \ 
	python3-pip

RUN pip3 install --upgrade pip

WORKDIR /data_project

RUN pip3 install requirements.txt

ENTRYPOINT ["/bin/bash"]
