FROM golang:latest

RUN go get github.com/sqdron/squad-digitalocean

RUN go install github.com/sqdron/squad-digitalocean

# Run the golang-docker command when the container starts.
WORKDIR /go/bin/

ENTRYPOINT ./squad-digitalocean