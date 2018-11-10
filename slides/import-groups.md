## Import groups

PHP 7.0+

<pre class="fragment-replacement"><code class="hljs lang-php fragment fade-out" data-fragment-index="0">&lt;?php

namespace My\Project;

use function Some\Library\foo;
use function Some\Library\bar;
use function Some\Library\baz;
</code><code class="hljs lang-php fragment fade-in" data-fragment-index="0">&lt;?php

namespace My\Project;

use function Some\Library\{foo, bar, baz};</code></pre>

Note:

In PHP 7.0 and above, we can also use curly-braces to group multiple `use` statements.

In this case, instead of importing three functions from Some\Library separately, we can do it in one line.
