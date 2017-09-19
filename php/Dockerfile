FROM php:7.2-rc-fpm-alpine

LABEL maintainer="Eakkapat Pattarathamrong (overbid@gmail.com)"

RUN set -x \
        && deluser www-data \
        && addgroup -g 500 -S www-data \
        && adduser -u 500 -D -S -G www-data www-data

RUN docker-php-ext-install \
        sockets
