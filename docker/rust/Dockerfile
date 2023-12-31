ARG UID=1000

FROM rust:latest

# Set the UID as the user
RUN useradd --create-home --uid $UID user
USER user
# Set the working directory
WORKDIR /app

# Copy the source code into the container
COPY . .

# Build the application
RUN cargo build --release

# Set the entrypoint command
CMD ["./target/release/my_app"]
