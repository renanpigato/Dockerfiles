FROM php:5.6-apache

# Create a php config file
#COPY config/php.ini /usr/local/etc/php/

# Install any needed extensions
RUN docker-php-ext-install pdo pdo_mysql \
    && docker-php-ext-install session \
    && docker-php-ext-install calendar 

# Enable mod_rewrite on apache
RUN a2enmod rewrite enable

# Make port 80 available to the world outside this container
EXPOSE 80

