# Use the official Golang base image
FROM golang:latest

# Set the UID as an argument to use as the user
ARG UID=1000

# Set default configurations
ENV GO111MODULE=on \
    CGO_ENABLED=0 \
    GOOS=linux \
    GOARCH=amd64 \
    UID=${UID}

# Set the working directory
WORKDIR /app

# Copy the source code to the working directory
COPY . .

# Build the application
RUN go build -o app .

# Set the entry point
ENTRYPOINT ["./app"]
