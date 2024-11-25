# Development

## Laragon

Laragon can be used for development but be sure you use the current PHP and MySQL versions as Laragon ships with older versions of PHP and MySQL.

## Laravel Sail

You need to install and start docker to use Laravel Sail.

Start Sail: `./vendor/bin/sail up`

Start Sail on Windows: 

1. `wsl`
2. `./vendor/bin/sail up` (You need to have WSL and Docker installed)

## Static Analysis

./vendor/bin/phpstan analyse

Windows: Run ./vendor/bin/phpstan.bat analyse in Powershell

## Testing

`php artisan test`

## Release

* `npm install`

* `npm run build`