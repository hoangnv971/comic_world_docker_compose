FROM php:8.1-fpm
COPY --from=composer:latest /usr/bin/composer /usr/local/bin/composer
RUN pecl install xdebug
RUN docker-php-ext-enable xdebug
RUN docker-php-ext-install pdo pdo_mysql

RUN apt-get update && apt-get install -y \
    git \
    zip \
    curl \
    sudo \
    unzip \
    libzip-dev \
    libicu-dev \
    libbz2-dev \
    libpng-dev \
    libjpeg-dev \
    libmcrypt-dev \
    libreadline-dev \
    libfreetype6-dev \
    g++

