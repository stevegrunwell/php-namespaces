### Importing namespaces

Import namespaces with the `use` keyword:

```php
<?php

namespace SteveGrunwell\PhpNamespaces;

use Ramsey\Uuid\Uuid;

function generateUuid(): string
{
    return Uuid::uuid4();
}
```

Note:

Instead, we can import namespaces with the "use" keyword.

Adding that "use" statement basically says "import Ramsey\Uuid\Uuid" and make it available as "Uuid".
