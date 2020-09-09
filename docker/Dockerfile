FROM nvidia/cuda:9.0-cudnn7-runtime-ubuntu16.04

# RUN 'echo'
# RUN apt-get update 
# RUN apt-get install -y  wget \
# 			vim \
# 			bzip2 \ 
# 			nano  \
# 			software-properties-common

RUN apt update && apt install software-properties-common && apt-get update && apt-get install -y --no-install-recommends \
    python3.7 \
    python3-pip \
    && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*
    
#RUN apt-get install -y software-properties-common
#RUN add-apt-repository ppa:deadsnakes/ppa

#RUN apt-get install \
#	python3.6 \ 
#	python3-pip

#RUN pip3 install --upgrade pip

# RUN apt install -y software-properties-common
# RUN add-apt-repository ppa:deadsnakes/ppa
# RUN apt-get update
# RUN apt-get install -y python3.6 | python3.6 -m pip install --upgrade pip
# # RUN apt-get install -y python3-pip
# # RUN python3.6 -m pip install --upgrade pip
# RUN python3.6 -m pip install -r requirements.txt


WORKDIR /data_project



ENTRYPOINT ["/bin/bash"]
