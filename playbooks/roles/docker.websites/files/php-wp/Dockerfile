FROM php:7.1-apache
RUN a2enmod rewrite && apt-get update && apt-get install -y libmcrypt-dev libfreetype6-dev libjpeg62-turbo-dev libpng-dev \
    &&docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ \
    && docker-php-ext-install mysqli pdo_mysql mcrypt gd
