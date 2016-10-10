FROM golang:latest

RUN go get github.com/sqdron/squad-auth-provider

RUN go install github.com/sqdron/squad-auth-provider

ADD connect.json /go/connect.json
ADD app.json /go/app.json

# Run the golang-docker command when the container starts.
ENTRYPOINT /go/bin/squad-auth-provider

EXPOSE 8080