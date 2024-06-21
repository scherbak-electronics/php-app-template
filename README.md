# PHP Application Template

This is as minimal as possible PHP application template designed to provide a basic project structure with Composer autoloading configured. It is ideal for super small minimalistic projects or scripts that require a clean, ultra-minimal setup with the capability to expand as needed.

## Features

- **Minimal Setup**: Only two files (`composer.json` and `main.php`) are initially present.
- **Composer Autoloading**: PSR-4 autoloading is configured, ready for you to add classes under the `src/` directory.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

You need to have Composer installed on your system to work with this project template. You can download and install Composer by following the instructions on the [official Composer website](https://getcomposer.org/download/).

### Installing

To start a new project based on this template, run the following command:

```bash
composer create-project scherbak-electronics/php-app-template path/to/your-new-project
```

### Structure
- `src/`: Directory where your PHP classes should be placed (following the `App\` namespace).
- `main.php`: A simple PHP script to demonstrate the setup. Modify or expand it as needed. To facilitate direct execution of the script from the command line, please include the shebang line `#!/usr/bin/env php` at the beginning of this file.
### Usage
After installation, you can start adding your PHP classes in the `src/` directory. For example, to add a new class `Example`, create a file `src/Example.php` with the following content:

```php
<?php
namespace App;

class Example {
    public function sayHello() {
        return "Hello from Example class!";
    }
}
```

You can then use this class in your `main.php` file:

```php
<?php
require __DIR__ . '/vendor/autoload.php';

use App\Example;

$example = new Example();
echo $example->sayHello();
```

To run your script, use:

```bash
php main.php
```

### Contributing
Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

### License
This project is open-sourced under the MIT License, but there is no LICENSE file for details, sorry.
