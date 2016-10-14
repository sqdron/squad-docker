FROM golang:latest

RUN go get github.com/sqdron/squad-gateway

RUN go install github.com/sqdron/squad-gateway

# Run the golang-docker command when the container starts.
ENTRYPOINT /go/bin/squad-gateway

# http server listens on port 8080.
EXPOSE 8080