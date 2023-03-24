FROM php:8.2-fpm

# Install extensions
RUN apt-get update -y && \
    apt-get install -y libmcrypt-dev && \
    apt-get install -y apt-utils zip unzip && \
    apt-get install -y nano && \
    apt-get install -y libzip-dev libpq-dev && \
    docker-php-ext-install pdo_mysql bcmath && \
    docker-php-ext-install zip && \
    rm -rf /var/lib/apt/lists/*

# Install Composer
COPY --from=composer:latest /usr/bin/composer /usr/local/bin/composer
