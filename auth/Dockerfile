# Set the working directory
WORKDIR /app

# Copy the current directory contents into the container
COPY ./auth/ .  # Ensure the correct path is used

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Make port 3002 available to the world outside this container
EXPOSE 3002

# Define the command to run your application
CMD ["python", "auth_service.py"]
