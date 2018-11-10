### Overloading

```php
function doSomethingDestructive()
{
    // We don't really want to do this.
}
```

```php
namespace Tests;

function doSomethingDestructive()
{
    // Just pretend, don't *actually* do it!
}
```
<!-- .element: class="fragment" -->

Note:

Because PHP will select the matching function in the current namespace before falling back to the global namespace, we can rewrite functions as necessary to change their behavior.

It's not something you should do often, but can be helpful when testing something that otherwise isn't using namespaces (like WordPress).
