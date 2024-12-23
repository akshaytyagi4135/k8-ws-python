# Use the official Python base image
FROM python:3.9-slim

# Set the working directory
WORKDIR /app

# Copy the service files into the container
COPY ./inventory_service/ /app/
COPY requirements.txt /app/
# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port for the service
EXPOSE 8082

# Set the default command to run the inventory service
CMD ["python", "inventory_app.py"]
