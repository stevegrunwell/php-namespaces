### Fallback

**Functions + constants** will fall back to the global namespace if not defined:

```php
namespace App;

// If App\doSomething() is undefined, call \doSomething().
doSomething();
```
<!-- .element: class="fragment" -->

<!-- .element: class="fragment" --> **Classes** will not fall back to the global namespace.
