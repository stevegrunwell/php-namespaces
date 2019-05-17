## `__NAMESPACE__`

<pre class="fragment-replacement"><code class="hljs lang-php fragment fade-out" data-fragment-index="0">&lt;php

namespace MyPlugin\Settings;

function register_settings() {
    // ...
}

add_action( 'init', __NAMESPACE__ . '\register_settings' );</code><code class="hljs lang-php fragment fade-in" data-fragment-index="0">&lt;php

namespace MyPlugin\Settings;

function register_settings() {
    // ...
}

add_action( 'init', 'MyPlugin\Settings\register_settings' );</code></pre>

Note:

If you need to get the fully-qualified name for something in your current namespace, the NAMESPACE magic constant is really handy.

For instance, WordPress actions and filters are relative to the global namespace, so if we want to hook our "register_settings" function into the "init" action, we need to give the qualified function name.
