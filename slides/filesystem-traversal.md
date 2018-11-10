### Analogy Time!

<p class="fragment-replacement">Getting to <code class="fragment fade-out" data-fragment-index="3">/var/www/html</code><code class="fragment fade-in" data-fragment-index="3">\var\www\html</code>:

<pre class="fragment-replacement fragment" data-fragment-index="0"><code class="hljs shell fragment fade-out" data-fragment-index="3">/var/www $ cd html</code><code class="hljs lang-php fragment fade-in" data-fragment-index="3">namespace var\www

html\some_func(); // Unqualified function name</code></pre>

<pre class="fragment-replacement fragment" data-fragment-index="1"><code class="hljs shell fragment fade-out" data-fragment-index="3">/var     $ cd www/html</code><code class="hljs lang-php fragment fade-in" data-fragment-index="3">namespace var

www\html\some_func(); // Qualified function name</code></pre>

<pre class="fragment-replacement fragment" data-fragment-index="2"><code class="hljs shell fragment fade-out" data-fragment-index="3">/etc     $ cd /var/www/html</code><code class="hljs lang-php fragment fade-in" data-fragment-index="3">namespace etc

\var\www\html\some_func(); // Fully-qualified function name</code></pre>

Note:

Think of namespaces like you would filesystem paths: we can reference them relative to our current position or from the filesystem root.

Imagine the filesystem root as the global namespace — everything is relative to that.
