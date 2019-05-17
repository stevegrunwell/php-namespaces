### Where does it go?

Namespaces must be defined before any other code in the file!

```php
<?php

namespace My\Namespace;

// Here comes the awesome!
```

<!-- .element: class="fragment" --> One exception: `declare()`

Note:

The namespace declaration should be the first thing in your file after the opening <?php tag. Think of it as setting the context for the rest of the file.

Putting anything before it will cause a fatal error.

One exception, though: the declare() construct, which helps set the file syntax rules.
