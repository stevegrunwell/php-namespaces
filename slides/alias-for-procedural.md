### More Aliases

```php
namespace MyPlugin\Updater;

use MyPlugin\Settings as Settings;

function checkForUpdates() {
    $product_key = Settings\get_value( 'product_key' );

    // ...
}
```

Note:

If you're writing procedural code, aliases can be helpful if you need to import a bunch of functions.

Typically how I write WP plugins
