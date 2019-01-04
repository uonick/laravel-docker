ARG PHP_VERSION
FROM php:${PHP_VERSION}

# imagick
RUN apt-get update && apt-get install -y \
    libmagickwand-dev --no-install-recommends
RUN pecl install imagick && docker-php-ext-enable imagick

# zip
RUN apt-get install -y zlib1g-dev

# xml
RUN apt-get install libxml2-dev

# extensions
RUN docker-php-ext-install pdo_mysql
RUN docker-php-ext-install mysqli && docker-php-ext-enable mysqli
RUN docker-php-ext-install json
RUN docker-php-ext-install iconv
RUN docker-php-ext-install mbstring
RUN docker-php-ext-install opcache
RUN docker-php-ext-install bcmath
RUN docker-php-ext-install tokenizer
RUN docker-php-ext-install ctype
