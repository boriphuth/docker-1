############################################################
# Dockerfile to build Nginx Installed Containers
# Based on Ubuntu
############################################################

# Set the base image to Ubuntu
FROM ubuntu

# File Author / Maintainer
MAINTAINER Maintaner Name


# Update the repository
RUN apt-get update

# Install necessary tools
RUN apt-get install -y  wget net-tools

# Install Nginx
RUN apt-get install -y nginx  

# Remove the  Nginx configuration file
RUN rm -v /etc/nginx/nginx.conf

# Copy a configuration file from the current directory
ADD nginx.conf /etc/nginx/


# Expose ports
EXPOSE 80

# Set the default command to execute
# when creating a new container
CMD service nginx start
