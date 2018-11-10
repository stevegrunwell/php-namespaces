### General rule of thumb

When referencing a core PHP class, it might be best to use the leading backslash.

```php
try {
    $object = new \stdClass;

    doSomething($object);
} catch (\OutOfRangeException $e) {
    // ...
}
```

Note:

This is more personal preference, but a common practice is to keep the leading backslash for global, core classes.

This makes it clear that we're referencing the OutOfRangeException that's defined as part of the SPL, not a custom exception somewhere in our app.
