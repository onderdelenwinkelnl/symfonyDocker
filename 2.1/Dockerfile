FROM phpdockerio/php72-fpm

LABEL Name="Fiyo" Version="1.0"

ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update \
    && apt-get -y install \
        apt-utils \
        unzip \
        zip \
        git \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*

RUN apt-get update \
    && apt-get -y --no-install-recommends install \
        php7.2-sqlite3 \
        php-memcached \
        php7.2-xmlrpc \
        php7.2-mysql \
        php7.2-pgsql \
        php-imagick \
        php-mongodb \
        php7.2-odbc \
        php7.2-soap \
        php7.2-intl \
        php-xdebug \
        php-redis \
        php-yaml \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*

    WORKDIR /var/www/html
