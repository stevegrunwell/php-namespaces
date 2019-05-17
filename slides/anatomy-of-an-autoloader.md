### Anatomy of an Autoloader

How does an autoloader work?

<pre class="hljs lang-php"><code>spl_autoload_register( function ( string $classname ) {</code><code class="fragment" data-fragment-index="0">    // Replace backslashes with forward slashes.
    $classname = str_replace( '\\', '/', $class );</code><code class="fragment" data-fragment-index="1">
    // Create a system filepath.
    $filename  = __DIR__ . '/src/' . $classname . '.php';</code><code class="fragment" data-fragment-index="2">
    // Include the file if it exists.
    if ( file_exists( $filename ) ) {
        include_once $filename;
    }</code><code>} );</code></pre>

Note:

You don't have to use a Composer-generated autoloader, especially if you're distributing your code!

Register autoloader callbacks with `spl_autoload_register()`; this callback which will be called when a referenced class doesn't exist.

Clean up the class name so it matches the filesystem pattern. This can be as complicated as you need it to be.

Then, if the resolved filename exists, include it!

This is a very basic example of how autoloaders work — Composer does a lot more to make things as easy as possible:
