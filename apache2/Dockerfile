FROM httpd:alpine

LABEL maintainer="Eakkapat Pattarathamrong (overbid@gmail.com)"

RUN set -x \
        && addgroup -g 500 -S core \
        && adduser -u 500 -D -S -G core core \
        && chown -R core: /usr/local/apache2

COPY ./httpd.conf /usr/local/apache2/conf/httpd.conf
COPY ./www.conf /usr/local/etc/php-fpm.d/www.conf
