# Base image: PHP 7.4 dengan Apache
FROM php:7.4-apache

# Instal ekstensi PostgreSQL untuk PHP 7.4
# php:7.4-apache berbasis Debian Buster, yang repositorinya masih aktif
RUN apt-get update && \
    apt-get install -y libpq-dev && \
    rm -rf /var/lib/apt/lists/* && \
    docker-php-ext-install pdo_pgsql pgsql