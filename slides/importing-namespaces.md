### Importing namespaces

Import namespaces with the `use` keyword:

<pre class="fragment-replacement"><code class="hljs lang-php fragment fade-out" data-fragment-index="0">namespace SteveGrunwell\PhpNamespaces;

function generateUuid(): string
{
    return \Ramsey\Uuid\Uuid::uuid4();
}</code><code class="hljs lang-php fragment fade-in" data-fragment-index="0">namespace SteveGrunwell\PhpNamespaces;

use Ramsey\Uuid\Uuid;

function generateUuid(): string
{
    return Uuid::uuid4();
}</code></pre>

Note:

Instead, we can import namespaces with the "use" keyword.

Adding that "use" statement basically says "import Ramsey\Uuid\Uuid" and make it available as "Uuid".
