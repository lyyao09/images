FROM golang:1.13.0
RUN mkdir -p /go/src/github.com/projectcalico/ && \
    cd /go/src/github.com/projectcalico/ && \
    git clone https://github.com/projectcalico/node.git && \
    cd node && \
    git checkout 06a613c127bd1a25f3963fc944aed66f2f837b6e && \
    cd cmd/calico-node/ && \
    go build
