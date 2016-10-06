# AvoidCommonPasswords plugin for CakePHP

## Installation

You can install this plugin into your CakePHP application using [composer](http://getcomposer.org).

The recommended way to install composer packages is:

```
composer require your-name-here/AvoidCommonPasswords
```

## Usage

First load the component

```php
$this->loadComponent('AvoidCommonPasswords.AvoidCommonPasswordCheck');
```

.. and then check the password ...

```php
if ( $this->AvoidCommonPasswordCheck->check($fancyPassword) ) {
    echo 'Go one, password looks fine';
} else {
    echo 'Please use another password';
}
```

... finished.