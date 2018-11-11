```php
# In some library or framework:
function doSomething(string $foo): bool
{
    // Does something, presumably.
}
```

```php
# In your code:
function doSomething(int $bar, array $baz): array
{
    // Not to be confused with the other one.
}
```
<!-- .element: class="fragment" -->

Note:

Let's say we have a function, doSomething(), defined somewhere else.

Now, our codebase introduces a function with the same name, and we're at an impasse, since both of these functions are defined in the GLOBAL namespace
