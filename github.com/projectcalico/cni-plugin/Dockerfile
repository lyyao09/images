  
FROM golang:1.13.0
RUN mkdir -p /go/src/github.com/projectcalico/ && \
    cd /go/src/github.com/projectcalico/ && \
    git clone https://github.com/projectcalico/cni-plugin.git && \
    cd cni-plugin && \
    git checkout a11fe45df62f2252cca484a1fd2ecd4a324f6ac5 && \
    cd cmd/calico/ && \
    go build
