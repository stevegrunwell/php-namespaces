<!-- .slide: data-class="has-dark-background" data-background="resources/galaxy-brain3.jpg" data-background-size="cover" data-background-position="center top" -->

<pre class="fragment-replacement"><code class="hljs lang-php fragment fade-out" data-fragment-index="0">class MyPlugin {
  public function hello_world() {
    echo 'Hello, World!';
  }
}

(new MyPlugin)->hello_world();</code><code class="hljs lang-php fragment fade-in" data-fragment-index="0">class MyPlugin {
  public static function hello_world() {
    echo 'Hello, World!';
  }
}

MyPlugin::hello_world();</code></pre>

Note:

The next step WordPress developers often take is doing this, making the function a method in a class.

They might even go as far as making them static methods, since we're not really doing OOP, so we don't have to instantiate them.

These are simply old, hacky workarounds for what we're here to talk about: namespaces.
