# adminpanel-laravel

Please check the official laravel installation guide for server requirements before you start. [Official Documentation](https://laravel.com/docs/5.6/installation#installation)


Clone the repository

    git clone https://github.com/Jinandra/adminpanel-laravel.git

Switch to the repo folder

    cd adminpanel-laravel

If you have linux system, you can execute the command below only in your project root

    1) sudo chmod -R 777 install.sh
    2) ./install.sh

If you have windows system, you can run Artisan Command for database setup, connection and configuration.

    php artisan install:app

Generate a new application key

    php artisan key:generate

Install Passport

    php artisan passport:install

Run the database migrations (**Set the database connection in .env before migrating**)

    php artisan migrate

Run the database seeders

    php artisan db:seed

Install the javascript dependencies using npm

    npm install

Compile the dependencies

    npm run development

For generating the files of unisharp file manager

    php artisan vendor:publish --tag=lfm_public

For linking storage folder in public

    php artisan storage:link

Start the local development server

    php artisan serve


You can now access the server at http://localhost:8000

**Command list**

    git clone https://github.com/Jinandra/adminpanel-laravel.git
    cd adminpanel-laravel
    cp .env.example .env
    composer install
    npm install
    npm run development
    php artisan storage:link
    php artisan key:generate
    php artisan passport:install
    php artisan vendor:publish --tag=lfm_public
    php artisan migrate
    php artisan passport:install

## Please note

- To run test cases, add SQLite support to your php

## Other Important Commands
- To fix php coding standard issues run - composer format
- To perform various self diagnosis tests on your Laravel application. run - php artisan self-diagnosis
- To clear all cache run - composer clear-all
- To built Cache run - composer cache-all
- To clear and built cache run - composer cc

## Logging In

`php artisan db:seed` adds three users with respective roles. The credentials are as follows:

* Administrator: `admin@admin.com`
* Backend User: `executive@executive.com`
* Default User: `user@user.com`

Password: `1234`

## Issues

If you come across any issues please report them [here](https://github.com/Jinandra/adminpanel-laravel/issues).