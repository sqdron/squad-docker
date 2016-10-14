FROM golang:latest

RUN go get github.com/sqdron/squad-oauth

RUN go install github.com/sqdron/squad-oauth

# Run the golang-docker command when the container starts.
WORKDIR /go/bin/

ENTRYPOINT ./squad-oauth

EXPOSE 5002