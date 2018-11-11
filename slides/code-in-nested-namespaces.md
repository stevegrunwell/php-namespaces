### In nested namespaces

```php
<?php

namespace App;

$event = new Events\SomeEvent; // \App\Events\SomeEvent
```

<!-- .element: class="fragment" --> **Pro-Tip:** There's no `../` traversal

Note:

We can also reference nested namespaces, relative to our current namespace. This is a **qualified** name.

Note that we can't work our way backwards — there's no ../ directory traversal
