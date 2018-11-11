### Overloading

```php
namespace App;

function createPost(array $args = []): Post
{
    $post = new Post($args);
    $post->created_at = time();
    $post->save();

    return $post;
}
```

```php
namespace Tests;

import function App\createPost;

class PostTest extends TestCase
{
    public function testStoresCreatedAtTimestamp()
    {
        $this->assertEquals(time(), createPost()->created_at);
    }
}
```
<!-- .element: class="fragment" -->

Note:

Because PHP will select the matching function in the current namespace before falling back to the global namespace, we can rewrite functions as necessary to change their behavior.

In this case, we might test that the current timestamp gets stored in the post's "created_at" property, but we don't have a way of controlling PHP's time() function.

It's not something you should do often, but can be helpful when testing something that otherwise isn't using namespaces (like WordPress).
