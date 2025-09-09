FROM php:8.2-fpm

RUN apt-get update && apt-get install -y \
    git unzip zip libonig-dev libxml2-dev libzip-dev curl \
    && docker-php-ext-install pdo_mysql mbstring zip exif pcntl bcmath xml

COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

WORKDIR /var/www/html

COPY . .

EXPOSE 9000

CMD ["php-fpm"]
