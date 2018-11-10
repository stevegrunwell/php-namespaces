### Using Aliases

<pre class="fragment-replacement"><code class="hljs lang-php fragment fade-out" data-fragment-index="0">&lt;?php

namespace App\Http;

use Some\Framework\Controller;

class Controller extends Controller
{
    😵
}</code><code class="hljs lang-php fragment fade-in" data-fragment-index="0">&lt;?php

namespace App\Http;

use Some\Framework\Controller as BaseController;

class Controller extends BaseController
{
    😎
}</pre>

Note:

When we import a namespace, we're occupying that name within our current namespace. What do we do if, for instance, we're writing a Controller class that extends a different Controller?

Using the "as" keyword, we can assign a different name to the imported namespace.
