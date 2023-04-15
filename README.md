# docker-lemp
A base LEMP stack

1. Download or git this repo
1. Download your prefered Laravel version from https://github.com/laravel/laravel
1. Copy Laravel files into this folder
1. Copy `.env.example` to `.env` and complete with information
1. Create a `public` folder where your PHP application will work

Now run your application `docker-compose up -d`
1. Get inside container `docker-compose exec app bash`
1. Install composer running `composer install`
1. Generate a Laravel application key `php artisan key:generate`

See your application at `http://localhost:<APP_PORT>`
