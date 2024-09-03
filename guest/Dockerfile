# Start with a base image
FROM python:3.8-slim

# Set the working directory
WORKDIR /app

# Copy only the necessary files
COPY guest/guest_service.py /app/
COPY requirements.txt /app/

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Expose port 3001 to the outside world
EXPOSE 3001

# Define the command to run your application
CMD ["python", "guest_service.py"]
