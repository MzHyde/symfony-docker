FROM php:fpm

# git and unzip for composer installs
RUN apt-get update && apt-get install -y \
        git unzip \
    --no-install-recommends && rm -r /var/lib/apt/lists/*

# zip for composer installs
RUN apt-get update && apt-get install -y \
        libzip-dev \
    && docker-php-ext-install zip

ENV COMPOSER_HOME /tmp
ENV COMPOSER_VERSION 1.8.5
# Install Composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
