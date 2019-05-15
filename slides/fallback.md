### Fallback

**Functions + constants** will fall back to the global namespace if not defined:

```php
namespace App;

// If App\doSomething() is undefined, call \doSomething().
doSomething();
```
<!-- .element: class="fragment" -->

<!-- .element: class="fragment" --> <u>Classes</u> will not fall back to the global namespace.

Note:

Functions and constants will work a little differently than classes: if a function/constant isn't defined in the current namespace, PHP will fall back to the global namespace. If it's not defined there, _then_ we get an error.

Classes will not fall back — they must either be imported or exist in the current namespace.
