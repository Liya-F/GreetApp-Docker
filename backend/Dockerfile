# Use the official Python image from the Docker Hub
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the requirements file into the container at /app
COPY requirements.txt /app/

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the backend folder contents into the container at /app
COPY . /app

# Expose port 5000 to the outside world
EXPOSE 5000

# Command to run the backend server
CMD ["python", "/app/app.py"]
