### Using Aliases

<pre class="fragment-replacement"><code class="hljs lang-php fragment fade-out" data-fragment-index="0">&lt;?php

namespace SteveGrunwell\MyTheme;

use SomeTheme\Widget;

class Widget extends Widget
{
    😵
}</code><code class="hljs lang-php fragment fade-in" data-fragment-index="0">&lt;?php

namespace SteveGrunwell\MyTheme;

use SomeTheme\Widget as BaseWidget;

class Widget extends BaseWidget
{
    😎
}</pre>

Note:

When we import a namespace, we're occupying that name within our current namespace. What do we do if, for instance, we're writing a child theme and want to write a Widget class to extend a class defined in the parent theme?

Using the "as" keyword, we can assign a different name to the imported namespace.
