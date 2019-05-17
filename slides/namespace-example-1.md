```php
# In some library or framework:
function do_something( string $foo ): bool
{
    // Does something, presumably.
}
```

```php
# In your code:
function do_something( int $bar, array $baz ): array
{
    // Not to be confused with the other one.
}
```
<!-- .element: class="fragment" -->

Note:

What do I mean by name collisions?

Let's say we have a function, do_something(), defined somewhere else.

Now, our codebase introduces a function with the same name, and we're at an impasse, since both of these functions are defined in the GLOBAL namespace
