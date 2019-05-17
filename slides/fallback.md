### Fallback

<u>Functions</u> + <u>constants</u> will fall back to the global namespace if not defined:

```php
namespace MyPlugin;

// Fall back to get_option() in the global namespace
$option = get_option( 'some-option' );
```

Note:

Functions and constants will work a little differently than classes: if a function/constant isn't defined in the current namespace, PHP will fall back to the global namespace. If it's not defined there, _then_ we get an error.
