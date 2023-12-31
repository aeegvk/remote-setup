# Use the official PHP image as the base image
FROM php:7.4-cli

# Set the UID argument (default to 1000 if not provided)
ARG UID=1000

# Add a new user with the provided UID
RUN adduser --disabled-password --gecos "" --uid $UID appuser

# Set the working directory to /app
WORKDIR /app

# Copy the application code to the container
COPY . /app

# Set the user to appuser
USER appuser

# Run your PHP application
CMD [ "php", "index.php" ]
