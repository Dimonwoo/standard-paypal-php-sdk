[![Generic badge](https://img.shields.io/github/last-commit/ewertondaniel/paypal-standard-php-sdk)](https://github.com/EwertonDaniel/paypal-standard-php-sdk)
[![Generic badge](https://img.shields.io/badge/stable-v1.0.1-blue.svg)](https://github.com/EwertonDaniel/paypal-standard-php-sdk)
[![GitHub license](https://img.shields.io/github/license/ewertondaniel/paypal-standard-php-sdk)](https://github.com/Naereen/StrapDown.js/blob/master/LICENSE)
[![Twitter](https://img.shields.io/twitter/follow/dsrewerton?style=social)](https://twitter.com/dsrewerton)

# PayPal Standard PHP SDK

_This library provides developers with a simple set of bindings to help you
integrate [PayPal Standard] (https://developer.paypal.com/home) to a website
and start receiving payments._

## 🛠 Requirements

`php >= 8.1`

`guzzlehttp/guzzle >= 7.0.1`

`echosistema/simple-http-request" >= 1.0.1`

📢 **Coming soon package to `PHP versions < 8.1`.**

## 💻 Installation

First time using PayPal? Create your PayPal account
in [PayPal](https://www.paypal.com/br/webapps/mpp/account-selection), if you don’t have one already.

Download [Composer](https://getcomposer.org/) if not already installed

On your project directory run on the command line `"composer require ewertondaniel/paypal-standard-php-sdk"`
for `PHP 8.1`;

That's it! **PayPal Standard PHP SDK** has been successfully installed!

## 🧑‍💻 Examples

### 🔓 Getting authorization

```php

use EwertonDaniel\PayPal\Auth;

  /**
   * Brazilian CPF and Phone Number can be only numbers or with default mask;
   * The email and phone number fields are optional;
   */
  
        $authentication = new Auth($client_id, $client_secret, $is_production);
        $authentication->getScopes();
        $authentication->getAccessToken();
        $authentication->getTokenType();
        $authentication->getAppId();
        $authentication->getExpiresIn();
        $authentication->getNonce();

```

## 📖 Documentation

### 🔗 Visit the PayPal for further information regarding:

[PayPal REST APIs Documentation](https://developer.paypal.com/api/rest/)
