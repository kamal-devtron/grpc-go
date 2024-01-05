FROM golang:1.20 AS build-env
WORKDIR /
COPY . .
RUN go mod tidy
WORKDIR /
RUN go build .
EXPOSE 8000
CMD ["./kamal"]