ARG UID=1000

FROM python:3.9

# Set the user with the provided UID
RUN useradd -m -u $UID appuser

# Set the working directory
WORKDIR /app

# Copy the requirements file
COPY requirements.txt .

# Install the Python dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the application code
COPY . .

# Set the user as the owner of the application code
RUN chown -R appuser:appuser /app

# Switch to the appuser
USER appuser

# Specify the command to run the application
CMD [ "python", "app.py" ]
