### What is Composer?

Package management tool for PHP

```sh
$ composer require ramsey/uuid
```
<!-- .element: class="fragment" -->

```sh
$ composer install
```
<!-- .element: class="fragment" -->

[![The Composer project logo](resources/composer.png)](https://getcomposer.org)
<!-- .element: class="seamless" -->

Note:

If you haven't used it before, Composer is the de facto package management tool for PHP. If you're familiar with npm or yarn, it's similar in a lot of ways.

We're able to define the dependencies of our project, such as that UUID library. We can also set version constraints.

To install our dependencies, we can run `composer install` and Composer will pull in everything we need.
