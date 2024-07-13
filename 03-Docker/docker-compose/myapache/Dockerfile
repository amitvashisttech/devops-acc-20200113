# Base Image.
FROM ubuntu:xenial-20210416

# Owner Name
MAINTAINER Amit Vashist <amitvashist7@gmail.com>

# Update APT Repo
RUN apt-get update

# Install Apache Packages
RUN apt-get install apache2 -y 

# Custom Index Page
RUN echo "HELLO WORLD.!!!" > /var/www/html/hello.html

# Copy My Code. 
COPY index.html /var/www/html/

# EXPOSE the PORT 
EXPOSE 80

# Start Apache Service
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
