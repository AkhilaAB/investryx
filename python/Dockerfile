# Use an official Python runtime as a parent image
FROM python:3.12

# Set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# Set the working directory
WORKDIR /smerger

# Install dependencies
COPY requirements.txt /smerger/
RUN python -m pip install --upgrade pip && pip install -r requirements.txt

# Copy the project code into the container
COPY . /smerger/