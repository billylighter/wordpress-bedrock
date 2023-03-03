FROM php:8.2.0-fpm-alpine

RUN docker-php-ext-install mysqli pdo pdo_mysql && docker-php-ext-enable mysqli

ADD https://github.com/mlocati/docker-php-extension-installer/releases/latest/download/install-php-extensions /usr/local/bin/

RUN chmod +x /usr/local/bin/install-php-extensions && \
    install-php-extensions gd xdebug imagick \

# RUN docker-php-ext-install nd_mysqli pdo pdo_mysql && docker-php-ext-enable nd_mysqli
