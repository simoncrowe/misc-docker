FROM nvidia/cuda:9.0-cudnn7-devel-ubuntu16.04

RUN apt-get update && apt-get upgrade -y \
    && apt-get install -y apt-utils curl gnupg python python-dev python-pip unzip vim

RUN pip install numpy==1.11.0 tensorflow-gpu==1.12 nltk==3.2.3 \
    requests==2.16.5 mock==2.0.0 markdown==2.3 h5py==2.7.1
RUN python -m nltk.downloader punkt

ENV PYTHONPATH=/img2txt

#RUN curl -fsSL https://bazel.build/bazel-release.pub.gpg | gpg --dearmor > bazel.gpg && \
#    mv bazel.gpg /etc/apt/trusted.gpg.d/ && \
#    echo "deb [arch=amd64] https://storage.googleapis.com/bazel-apt stable jdk1.8" | tee /etc/apt/sources.list.d/bazel.list

#RUN apt-get update && apt-get install -y bazel-1.0.0 
