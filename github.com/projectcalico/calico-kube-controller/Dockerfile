FROM golang:1.13.0
RUN mkdir -p /go/src/github.com/projectcalico/ && \
    cd /go/src/github.com/projectcalico/ && \
    git clone https://github.com/projectcalico/kube-controllers.git && \
    cd kube-controllers && \
    git checkout ba8d74176df78d220d54de919145a04b900bbb21 && \
    cd cmd/kube-controllers/ && \
    go build
