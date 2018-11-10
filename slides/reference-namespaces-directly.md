### Fully-qualified class names

```php
<?php

namespace SteveGrunwell\PhpNamespaces;

function generateUuid(): string
{
    return \Ramsey\Uuid\Uuid::uuid4();
}
```

Note:

The first way to use namespaces is to use the fully-qualified class name.

Here, we're calling the Uuid::uuid4() method from the Ramsey\Uuid package. Note the leading backslash — that tells PHP this is relative to the global namespace.

It works, but it's kind of ugly, especially if the package namespace was longer.

**fully-qualified** name
