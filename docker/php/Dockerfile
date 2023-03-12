FROM php:8.2-fpm-alpine

RUN apk add --no-cache $PHPIZE_DEPS \
  bash \
&& pecl install mongodb \
&& docker-php-ext-enable mongodb \
&& curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

