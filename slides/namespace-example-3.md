```php
namespace SomeVendor\Package;

function doSomething(string $foo): bool
{
    // Does something, presumably.
}
```

```php
namespace MyName\MyApp;

function doSomething(int $bar, array $baz): array
{
    // Not to be confused with the other one.
}
```
<!-- .element: class="fragment" -->

Note:

Now we've added namespaces to both methods: SomeVendor\Package to the first one

and MyName\MyApp to the second.

These functions are now effectively named "SomeVendor\Package\doSomething" and "MyName\MyApp\doSomething"
