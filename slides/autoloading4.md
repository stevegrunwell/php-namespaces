### Autoloading (with Composer)

* <!-- .element: class="fragment" -->Multiple autoloading methods: `psr-4`, `psr-0`, `classmap`
* <!-- .element: class="fragment" -->Auto-include (`files`)
* <!-- .element: class="fragment" -->Development-only autoloading (`autoload-dev`)

Note:

The Composer autoloader supports a few different patterns — you can use path-based autoloading (like we've seen), specify where particular classes live (classmap)

We can also use `files` to auto-include files on every request.

We can also define things that should only be autoloaded in development dependencies, such as test dependencies or debug tools.
