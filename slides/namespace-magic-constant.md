## `__NAMESPACE__`

<pre class="fragment-replacement"><code class="hljs lang-php fragment fade-out" data-fragment-index="0">&lt;php

namespace DoofenschmirtzEvilInc\Plugininator;

add_action( 'init', __NAMESPACE__ . '\init' );</code><code class="hljs lang-php fragment fade-in" data-fragment-index="0">&lt;php

namespace DoofenschmirtzEvilInc\Plugininator;

add_action( 'init', '\DoofenschmirtzEvilInc\Plugininator\init' );</code></pre>

Note:

This magic constant is really handy if, for instance, you need to register a callable with something that lives in the global namespace.

When doing things like registering hooks within WordPress, the hooks are assumed to be relative to the *global* namespace, since WordPress doesn't have any concept of PHP namespaces.
