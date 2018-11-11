### Overloading

```php
namespace App;

function time(): int
{
    return 12345;
}
```

```php
namespace Tests;

import function App\createPost;

class PostTest extends TestCase
{
    public function testStoresCreatedAtTimestamp()
    {
        $this->assertEquals(12345, createPost()->created_at);
    }
}
```
<!-- .element: class="fragment" -->

Note:

If we define and load a time() function in the App namespace that returns a known value for our tests, we can assert that createPost() stored the value of time() in created_at.

It's not something you should do often (code smell, use DI instead), but can be helpful when testing something that otherwise isn't using namespaces (like WordPress).
