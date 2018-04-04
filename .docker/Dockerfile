FROM php:7.1.8-apache

MAINTAINER Colin Kier

COPY .docker/vhost.conf /etc/apache2/sites-available/laravel-docker.test.conf

RUN a2dissite 000-default.conf

RUN a2ensite laravel-docker.test.conf

WORKDIR /var/www/laravel-docker

RUN docker-php-ext-install mbstring pdo pdo_mysql
