### Defining constants

The `define()` function requires a fully-qualified namespace!

```php
namespace Starbucks;

define('ROAST_LEVEL', 'burned to a crisp');
```
<!-- .element: class="fragment" -->

```php
namespace GoodCoffeeShop;

define('ROAST_LEVEL', 'Full City');
```
<!-- .element: class="fragment" -->

```php
# Starbucks ruins everything!
PHP Notice:  Constant ROAST_LEVEL already defined in
/src/GoodCoffeeShop.php on line 5.
```
<!-- .element: class="fragment" -->
