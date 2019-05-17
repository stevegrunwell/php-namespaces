### composer.json

```json
{
    "autoload": {
        "psr-4": {
            "SteveGrunwell\\MyPlugin\\": "src/"
        }
    }
}
```

```php
SteveGrunwell\MyPlugin\Settings
#=> src/Settings.php

SteveGrunwell\MyPlugin\Views\UserConfig
#=> src/Views/UserConfig.php
```
<!-- .element: class="fragment" -->

Note:

The composer.json file contains any dependencies that your project has, as well as defining information about the project.

One important key is the "autoload" section, where you can specify where everything lives. There's also an "autoload-dev" that can specify things that should only be autoloaded in development configurations.

PSR-4 is a standard that expects the filesystem path to match the namespace structure, which improves code organization.
