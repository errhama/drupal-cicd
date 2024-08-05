# Use the official PHP image with Apache
FROM php:8.2-apache

# Install Drupal dependencies
RUN docker-php-ext-install pdo pdo_mysql mysqli

# Set the working directory
WORKDIR /var/www/html

# Copy the local code to the container
COPY ../  /var/www/html

# Set appropriate permissions
RUN chown -R www-data:www-data /var/www/html

# Expose the port
EXPOSE 80