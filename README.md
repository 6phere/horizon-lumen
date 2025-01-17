<p align="center"><img src="https://laravel.com/assets/img/components/logo-horizon.svg"></p>

<p align="center">
<a href="https://github.com/laravel/horizon/actions"><img src="https://github.com/laravel/horizon/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/horizon"><img src="https://img.shields.io/packagist/dt/laravel/horizon" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/horizon"><img src="https://img.shields.io/packagist/v/laravel/horizon" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/horizon"><img src="https://img.shields.io/packagist/l/laravel/horizon" alt="License"></a>
</p>

## Introduction

Changes introduced by Sixphere to adapt Horizon 5 to be used on Lumen 8.

Horizon provides a beautiful dashboard and code-driven configuration for your Laravel powered Redis queues. Horizon allows you to easily monitor key metrics of your queue system such as job throughput, runtime, and job failures.

All of your worker configuration is stored in a single, simple configuration file, allowing your configuration to stay in source control where your entire team can collaborate.

## Installation

1. If Redis is not installed, you have to install it

composer require illuminate/redis

2. Add the provider into bootstrap/app.php file

$app->register(Illuminate\Redis\RedisServiceProvider::class);

3. Require horizon-lumen by composer

composer require 6phere/horizon-lumen

4. Add the provider into bootstrap/app.php file

$app->register(Laravel\Horizon\HorizonServiceProvider::class);

3. Publish the config and assets

php artisan horizon:install


## Official Documentation

Documentation for Horizon can be found on the [Laravel website](https://laravel.com/docs/horizon).

## Contributing

Thank you for considering contributing to Horizon! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

Please review [our security policy](https://github.com/laravel/horizon/security/policy) on how to report security vulnerabilities.

## License

Laravel Horizon is open-sourced software licensed under the [MIT license](LICENSE.md).
