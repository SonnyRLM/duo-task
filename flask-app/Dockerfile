# Use Python 3.6 or later as a base image
FROM python:3.8
RUN apt-get update && apt-get install -y python3-pip
# Copy contents into image
COPY . . 
# Install pip dependencies from requirements
RUN pip3 install Flask==1.1.2 
# Set YOUR_NAME environment variable
ENV YOUR_NAME='TEAM4'
# Expose the correct port
EXPOSE 5500
# Create an entrypoint
ENTRYPOINT ["/usr/local/bin/python3", "app.py"]
