FROM php:7.2-apache

# Info obtained by DockerHub
RUN apt-get -y update \
&& apt-get install -y libicu-dev \
&& docker-php-ext-configure intl \
&& docker-php-ext-install intl

RUN docker-php-ext-install mysqli && docker-php-ext-enable mysqli   

COPY index.php /var/www/html