FROM php:7.4-fpm

RUN apt-get update && \
    apt-get install -y zip libzip-dev libpng-dev

RUN docker-php-ext-install mysqli pdo pdo_mysql gd zip

RUN pecl install xdebug-3.1.5 &&  \
    docker-php-ext-enable xdebug
