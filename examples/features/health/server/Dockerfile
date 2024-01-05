FROM golang:1.20 AS build-env
WORKDIR /go/src/github.com/kamal-devtron/grpc-go/server
COPY . .
RUN go mod tidy
WORKDIR /go/src/github.com/kamal-devtron/grpc-go/server
RUN go build .
EXPOSE 3000
CMD ["./server"]