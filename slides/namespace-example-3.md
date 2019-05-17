```php
namespace SomeVendor\Package;

function do_something( string $foo ): bool
{
    // Does something, presumably.
}
```

```php
namespace MyName\MyApp;

function do_something( int $bar, array $baz ): array
{
    // Not to be confused with the other one.
}
```
<!-- .element: class="fragment" -->

Note:

Now we've added namespaces to both methods: SomeVendor\Package to the first one

and MyName\MyApp to the second.

These functions are now effectively named "SomeVendor\Package\do_something" and "MyName\MyApp\do_something"
