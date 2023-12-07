FROM golang:latest

WORKDIR /go/src/app

# Copy the Go application source code from the host to the container's working directory
COPY app_files /go/src/app

# Initialize Go modules (if required)
RUN go mod init myapp

# Build the Go application inside the container
RUN go build -o myapp

EXPOSE 8080

CMD ["./myapp"]
