# Base Image
FROM python:3.11

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements file
COPY requirements.txt .

# Install the project dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the application code into the container
COPY . .


# Expose the port to the Flask application will be listening on
EXPOSE 5000


# Set environment varibles, if necessary
# ENV MY_ENV_VAR=value

# RUN the Flask application
CMD ["python", "app.py"]

