<!-- .slide: data-background-image="resources/paint-your-wagon.gif" data-background-size="cover" data-background-position="center" -->

```php
// The vendor-provided function:
SomeVendor\Package\doSomething($foo);

// A totally different function!
MyName\MyApp\doSomething($bar, $baz);
```

Note:

Since they have different names relative to the global namespace, PHP has no issues.

As far as PHP is concerned, we might as well have named them SomeVendor_Package_DoSomething() and MyName_MyApp_DoSomething().
