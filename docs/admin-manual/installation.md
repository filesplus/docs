---
sidebar_position: 1
---

# Installation

## Requirements

PHP 8.2

MySQL / MariaDB

nginx / apache

## Guide

1. `git clone https://github.com/filesplus/filesplus.git`

2. Set Environment variables in .env

2. `composer install --optimize-autoloader --no-dev`

3. `php artisan optimize`

4. `php artisan config:cache`

5. `php artisan route:cache`

6. `php artisan view:cache`

7. `php artisan migrate`

8. Open The Web Browser at the host address or run `php artisan filesplus:install`


TODO: `php artisan filesplus:scan`

TODO: command to check if all requirements are fulfilled, run be -> should work without composer install?


## The .env File Explained

* APP_ENV

* DEMO_MODE (bool) - will prevent any actions to files if enabled

* FILESPLUS_INSTALLED (bool)

### Database

* DB_CONNECTION
* DB_HOST
* DB_PORT
* DB_DATABASE
* DB_USERNAME
* DB_PASSWORD
