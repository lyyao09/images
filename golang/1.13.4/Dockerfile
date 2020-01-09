FROM golang:1.13.4

WORKDIR /go/src/k8s.io
RUN apt-get update \
    && apt-get install -y rsync \
    && git clone https://github.com/kubernetes/kubernetes.git \
    && apt-get clean
    
WORKDIR /go/src/k8s.io/kubernetes
