FROM golang:latest

RUN go get github.com/sqdron/squad-hub

RUN go install github.com/sqdron/squad-hub

# Run the golang-docker command when the container starts.
ENTRYPOINT /go/bin/squad-hub

# http server listens on port 8080.
EXPOSE 5001