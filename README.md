# Extended Laravel Logger

Extended Laravel Logger is a library for logging in Laravel, extending the functionality of the default logger by adding
the file path and line number to the context where the logger was called.

## Installation

You can install the package via Composer:

```bash
composer require vlsv/extended-laravel-logger
```

## Usage

Example of using the debug method:

```php
use Vlsv\ExtendedLaravelLogger\Log;

Log::debug('This is a debug message', ['additional' => 'context']);
```

The library provides methods for different logging levels: debug, info, notice, warning, error, critical, alert,
emergency.

### Additional Context

Each log automatically adds context, including the file path and line number.
