# Development

Filesplus is built with Laravel (PHP) and MySQL in the backend and React (bundled with Vite) in the frontend. If you are familiar with this stack, understanding the codebase should be quite easy.

## Development environment

### Laravel Herd

Laravel Herd can be used as a dev environment for Filesplus. However, you will need Herd Pro as Filesplus needs MySQL to work (or use a custom MySQL server).

### Laragon

Laragon can be used for development but be sure you use the current PHP and MySQL versions as Laragon ships with older versions of PHP and MySQL.

### Laravel Sail

You need to install and start docker to use Laravel Sail.

Start Sail: `./vendor/bin/sail up`

Start Sail on Windows: 

1. `wsl`
2. `./vendor/bin/sail up` (You need to have WSL and Docker installed)

## Static Analysis

`./vendor/bin/phpstan analyse`

Windows: Run `./vendor/bin/phpstan.bat analyse` in Powershell

## Javascript

* Prettier

## Testing

`php artisan test`

### Run Feature Tests only

`php artisan test --testsuite=Feature`

### Run Unit Tests only

`php artisan test --testsuite=Unit`

### Coverage Reports

`php artisan test --coverage-html tests/reports/coverage`

### vitest

wip

## Release

* `npm install`

* `npm run build`