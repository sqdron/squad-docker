FROM golang:latest

RUN go get github.com/sqdron/squad-hub
ADD config.json github.com/sqdron/squad-hub/config.json

RUN go install github.com/sqdron/squad-hub

ADD config.json /go/config.json

# Run the golang-docker command when the container starts.
ENTRYPOINT /go/bin/squad-hub

# http server listens on port 8080.
EXPOSE 5001