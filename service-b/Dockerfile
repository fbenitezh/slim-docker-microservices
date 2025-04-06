FROM php:8.2-fpm

WORKDIR /var/www/html

# Instalar extensiones necesarias
RUN docker-php-ext-install pdo pdo_mysql

# Composer (opcional si usas Slim)
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer
