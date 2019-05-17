### Autoloading

Only `include` the file when needed:

<pre class="fragment-replacement"><code class="hljs lang-php fragment fade-out" data-fragment-index="0">&lt;?php

// A life without autoloading
function generate_uuid() {
    require_once 'vendor/ramsey/uuid/src/Generator/RandomGeneratorInterface.php';
    require_once 'vendor/ramsey/uuid/src/Generator/UuidBuilderInterface.php';
    require_once 'vendor/ramsey/uuid/src/BinaryUtils.php';
    require_once 'vendor/ramsey/uuid/src/FeatureSet.php';
    require_once 'vendor/ramsey/uuid/src/Uuid.php';
    require_once 'vendor/ramsey/uuid/src/UuidFactory.php';
    // I stopped after going two levels deep!

    return Ramsey\Uuid\Uuid::uuid4();
}</code><code class="hljs lang-php fragment fade-in" data-fragment-index="0">&lt;?php

require_once 'vendor/autoload.php';

// Way better!
function generate_uuid() {
    return Ramsey\Uuid\Uuid::uuid4();
}</code></pre>

```json
{
    "autoload": {
        "psr-4": {
            "Ramsey\\Uuid\\": "src/"
        }
    }
}
```
<!-- .element: class="fragment" data-fragment-index="1" -->

Note:

Using an autoloader essentially tells PHP "here's how to find the code, please pull it in when I need it."

generate_uuid() function from earlier: we don't need to have this series require_once statements because the UUID package uses namespaces and populates its 'autoload' property in composer.json.
