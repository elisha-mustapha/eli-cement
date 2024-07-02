# Use the official PHP 8.1 Apache image as the base image
FROM php:8.2-apache-buster

# Set the working directory in the container (Contains the composer.json file)
WORKDIR /var/www/html/

# Enable Apache modules
RUN a2enmod rewrite

# Copy the application files to the container
COPY . /var/www/html/

# Setting file permissions to run Laravel
RUN chown -R www-data:www-data /var/www/html/