FROM php:8.3-fpm

WORKDIR '/app'

RUN apt-get update; \
    apt-get -y --no-install-recommends install \
        php8.3-pgsql \
        php8.3-psr; \
    apt-get clean; \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
