FROM golang:latest


## Copy the local package files to the container’s workspace.
COPY config.json $GOPATH/src/github.com/sqdron/squad-hub

RUN go install github.com/sqdron/squad-hub

# Run the golang-docker command when the container starts.
ENTRYPOINT /go/bin/squad-hub

# http server listens on port 8080.
EXPOSE 5001