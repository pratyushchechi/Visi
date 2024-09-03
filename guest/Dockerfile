# Dockerfile in /guest/
FROM python:3.8-slim

# Set the working directory
WORKDIR /app

# Copy the current directory contents into the container
COPY . .

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Make port 3001 available to the world outside this container
EXPOSE 3001

# Define the command to run your application
CMD ["python", "guest_service.py"]
