# 🍱 Bento for Laravel
Provides Bento mailer integration for Laravel.

## Requirements

* [PHP 8.0+](https://php.net/releases/)
* [Laravel 9.0+](https://www.laravel.com)
* [API Keys from Bentonow](https://www.bentono.com)

## Setup
First you can install the package via composer:
```bash
composer require bentonow/bento-laravel-sdk
```

Second publish the configuration file
```bash
php artisan vendor:publish --tag bentonow-laravel-sdk
```

Create a new mailer definition within your application's `config/mail.php` configuration file:
```php
'bento' => [
	'transport' => 'bento',
	],
```

Next visit your bento profile and generate your api keys.
Add the Api keys to your env and set your mail_mailer to use bento:
```dotenv
BENTO_PUBLISHABLE_KEY="{Publishable Key}"
BENTO_SECRET_KEY="{Secret Key}"
BENTO_SITE_UUID="{Site Key UUID}"
MAIL_MAILER="bento"
```

For additional information please refer to [Laravel Mail documenation](https://laravel.com/docs/9.x/mail)

## Support and Feedback

In case you find any bugs, submit an issue directly here in GitHub.

To get personalized support, please tweet @bento or email ~[jesse@bentonow.com](mailto:jesse@bentonow.com)~

Official API documentation is at [https://docs.bentonow.com](https://docs.bentonow.com)

## License

[The MIT License (MIT)](LICENSE.md)

## Authors

- [@aarondfrancis](https://github.com/aarondfrancis)
- [@ziptied](https://github.com/ziptied)