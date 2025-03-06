# Use an official Pyton runtime as the parent image
FROM python:3.7-slim

# Set the working directory in the container to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
ADD . /app

# Install any needed packages specified in requirements.txt [when the container image creation]
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# Make the container's port 5000 available to the outside world
EXPOSE 5000

# The ENTRYPOINT instruction in a Dockerfile specifies the main command that runs 
# when a container starts. It is typically used when you want your 
# container to act as an executable.
ENTRYPOINT [ "python" ]

# Run app.py using python when the container launches
CMD [ "app.py" ]