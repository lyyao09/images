FROM golang:1.13.0
RUN mkdir -p /go/src/github.com/projectcalico/ && \
    cd /go/src/github.com/projectcalico/ && \
    git clone https://github.com/projectcalico/node.git && \
    cd node && \
    git checkout d296a4e118245d0c2e038b42cbf016bda676c58d && \
    cd cmd/calico-node/ && \
    curl https://glide.sh/get | sh && \
    glide install
