# drupal/Dockerfile

# Use an official Drupal base image
FROM drupal:9.3-php7.4-apache

# Copy custom configuration files if needed
# COPY ./config/php.ini /usr/local/etc/php/

# Install PostgreSQL PHP extensions
RUN apt-get update && apt-get install -y libpq-dev \
    && docker-php-ext-install pdo pdo_pgsql

# Copy Drupal configuration files if needed
# COPY ./config/settings.php /var/www/html/sites/default/

# Set permissions if needed
# RUN chown -R www-data:www-data /var/www/html/

# Expose port 80 to allow Drupal to be accessed from the host
EXPOSE 80

