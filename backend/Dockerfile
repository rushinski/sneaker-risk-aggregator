# Takes the offical python:3.12-slim image from docker hub
FROM python:3.12-slim

# Sets what directory inside the container to place the code
WORKDIR /app

# Takes a file from my laptop and places it inside the image under the current WORKDIR path
COPY requirements.txt .

# At build time install every package listed in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Copys our whole project into /app because we set WORKDIR /app earlier
# The left "." is the folder on our laptop and the right "." is the current WORKDIR inside the image
COPY . .
