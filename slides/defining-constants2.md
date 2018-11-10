### Defining constants

<pre class="fragment-replacement"><code class="hljs lang-php fragment fade-out" data-fragment-index="0">namespace Starbucks;

define('Starbucks\ROAST_LEVEL', 'burned to a crisp');</code><code class="hljs lang-php fragment fade-in" data-fragment-index="0">namespace Starbucks;

define(__NAMESPACE__ . '\ROAST_LEVEL', 'burned to a crisp');</code></pre>

<pre class="fragment-replacement"><code class="hljs lang-php fragment fade-out" data-fragment-index="0">namespace GoodCoffeeShop;

define('GoodCoffeeShop\ROAST_LEVEL', 'Full City');</code><code class="hljs lang-php fragment fade-in" data-fragment-index="0">namespace GoodCoffeeShop;

define(__NAMESPACE__ . '\ROAST_LEVEL', 'Full City');</code></pre>

Note:

Instead, we should define our constants with explicit namespaces.

We can even use our handy NAMESPACE magic constant!
