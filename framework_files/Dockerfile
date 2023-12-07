# Use an official Golang runtime as a base image
FROM golang:latest

# Set the working directory inside the container
WORKDIR /go/src/app

# Copy the Go application source code from the host to the container's working directory
COPY ./framework_files/app_files /go/src/app

# Build the Go application inside the container
RUN go build -o myapp

# Expose a port (if your Go application listens on a specific port)
EXPOSE 8080

# Command to run the application when the container starts
CMD ["./myapp"]