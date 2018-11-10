### Autoloading

<pre class="fragment-replacement"><code class="hljs lang-php fragment fade-out" data-fragment-index="0">&lt;?php

App\User
App\Services\Twilio
App\Controllers\UserController</code><code class="hljs lang-php fragment fade-in" data-fragment-index="0">&lt;?php

App\User                       => src/User.php
App\Services\Twilio            => src/Services/Twilio.php
App\Controllers\UserController => src/Controllers/UserController.php</code></pre>

```json
{
    "autoload": {
        "psr-4": {
            "App\\": "src/"
        }
    }
}
```
<!-- .element: class="fragment" data-fragment-index="1" -->

Note:

When namespaces structure matches the filesystem structure, code can easily be easily autoloaded.

We tell Composer that the "App" namespace refers to src/, and it can guess paths from there.

Improves organization of code.
