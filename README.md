# PHP Environment Variables Manager

A simple library for managing environment variables in PHP.

## Usage

To use this library, simply create a `.env` file at the root of the project, following the model below (one variable per line):

```
DB_HOST=localhost
DB_USER=root
DB_PASS=pass
DB_NAME=database
DB_PORT=3307
```

```php
<?php

require 'vendor/autoload.php';

//LOAD ENVIRONMENT VARS FROM FILE ON ROOT
WilliamCosta\DotEnv\Environment::load(__DIR__);

//GET ENVIRONMENT VAR
echo getenv('DB_HOST');

```

## Requirements

This library needs PHP 7.0 or greater.
