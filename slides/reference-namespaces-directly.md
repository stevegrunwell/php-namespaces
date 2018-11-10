### Fully-qualified class names

```php
<?php

namespace App;

function getFeed(string $url): string
{
    $parser = new \Some\Library\Parser($url);

    // ...
}
```

Note:

The first way to use namespaces is to use the fully-qualified class name.

Here, we're calling the Uuid::uuid4() method from the Ramsey\Uuid package. Note the leading backslash — that tells PHP this is relative to the global namespace.

It works, but it's kind of ugly, especially if the package namespace was longer.

**fully-qualified** name
