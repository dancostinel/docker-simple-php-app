FROM php:8.2.0-fpm
RUN apt-get update && apt-get install apt-file -y && apt-file update && apt-get install vim -y --no-install-recommends \
        git \
        zlib1g-dev \
        libxml2-dev \
        libzip-dev \
        unzip \
    && docker-php-ext-install \
        zip \
        intl \
        mysqli \
        pdo pdo_mysql \
        ctype \
        iconv \
        session \
        simplexml

WORKDIR /var/www/html/app/