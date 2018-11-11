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

If we're referencing something in a totally different namespace, we can do so by using the **fully-qualified class name**, starting with a leading backslash.

Here, we're using the Parser class that lives in the Some\Library namespace.
