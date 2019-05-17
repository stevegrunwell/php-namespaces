### In the same namespace

```php
<?php

namespace MyPlugin;

$post = new Post; // \MyPlugin\Post
$user = new User; // \MyPlugin\User
```

Note:

If we're using code in the same namespace, it's automatically available to us.

If we're in the "App" namespace and have classes Post and User at the same level under the "App" namespace, we can work with them directly.

This is an **unqualified** name
