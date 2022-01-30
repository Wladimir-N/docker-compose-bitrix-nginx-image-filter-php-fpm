FROM php:7.4.27-fpm-alpine3.15
RUN apk add freetype-dev \
            libjpeg-turbo-dev \
            libpng-dev \
            zlib-dev && \
    docker-php-ext-configure gd --with-freetype \
                                --with-jpeg && \
    docker-php-ext-install gd \
                           mysqli \
                           opcache
