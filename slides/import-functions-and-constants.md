### Import functions and constants

PHP 5.6+

<pre class="fragment-replacement"><code class="hljs lang-php fragment fade-out" data-fragment-index="0">namespace MyPlugin\Updater;

use MyPlugin\Settings as Settings;

function check_for_updates() {
    $product_key = Settings\get_value( Settings\PRODUCT_KEY );

    // ...
}</code><code class="hljs lang-php fragment fade-in" data-fragment-index="0">namespace MyPlugin\Updater;

use function MyPlugin\Settings\get_value;
use const MyPlugin\Settings\PRODUCT_KEY;

function check_for_updates() {
    $product_key = get_value( PRODUCT_KEY );

    // ...
}</pre>

Note:

We can also explicitly import functions and constants into our namespace, using the 'function' or 'const' keywords after 'use'.

PHP 5.6+
