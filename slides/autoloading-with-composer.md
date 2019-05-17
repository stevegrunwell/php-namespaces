### Autoloading with Composer

Generated autoloader based on composer.json:

```php
require_once __DIR__ . '/vendor/autoload.php';
```

Note:

When installing Composer dependencies, the last step is generating an autoloader. Composer reads your composer.json file and the composer.json files of all of its dependencies to automatically build this file, which lives at vendor/autoload.php relative to your project root.

We can load this file into our app to have access to everything, automatically!

If there are files that don't fit PSR-4, you can also add them to "classmap" or "files" keys in your composer.json file to have them added to the autoloader.
