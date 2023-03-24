FROM php:8.2-fpm

# Install extensions
RUN docker-php-ext-install pdo_mysql bcmath

# Install Composer
COPY --from=composer:latest /usr/bin/composer /usr/local/bin/composer