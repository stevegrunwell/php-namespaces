### Fallback

<u>Classes</u> will not fall back to the global namespace.

```php
namespace MyPlugin;

$query = new WP_Query();
```

```sh
PHP Fatal error:
    Uncaught Error: Class 'MyPlugin\WP_Query' not found
```

<!-- .element: class="fragment" -->

Note:

Classes, on the other hand, will not fall back — they must either be imported or exist in the current namespace.
