### Autoloading

Autoloading gives your code super powers!

<pre class="hljs lang-php"><code>namespace App;</code><code class="hljs lang-php fragment" data-fragment-index="1">
use YourName\PartyAnimal\Parrot;
use YourName\PartyAnimal\Exceptions\PartyException;</code><code class="fragment" data-fragment-index="0">
require_once __DIR__ . '/vendor/autoload.php';</code><code class="fragment" data-fragment-index="1">
try {
    $partyParrot = new Parrot;
    $partyParrot->party();
} catch (PartyException $e) {
    error_log('Unable to party: ' . $e->getMessage());
}</code></pre>

Note:

If we write our code in a way that it can be autoloaded, other developers only need to include `vendor/autoload.php` to start using it!

No complex requires, no worrying about the order in which files load, just loading everything we need on-demand.
