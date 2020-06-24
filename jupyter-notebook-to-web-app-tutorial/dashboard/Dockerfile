# Use Ubuntu operating system
FROM ubuntu

# Create /app folder on docker container
WORKDIR /app

# Copy all the files from current folder to /app folder
COPY . /app

# Install Python and pip
RUN apt-get update && apt-get install -y \
    python3 \
    python3-pip

# Install Python dependancies from requirements.txt file    
RUN pip3 install -r requirements.txt

# By default Voilà uses port 8866
EXPOSE 8866

# Run voila when the cotainer is launched
# Note, you need to change dashboard.ipynb to your notebook name
CMD voila dashboard.ipynb