TwigTruncateBundle
==================

A Symfony2 bundle to include the [TwigTruncateExtension](https://github.com/dzango/TwigTruncateExtension) into your app. The TwigTruncateExtension allows you to truncate text while preserving HTML tags.

Installation
------------

Add the bundle to your app's `composer.json`:

```json
    "require": {
        "dzango/twig-truncate-bundle": "~1.0",
        ...
    }
```

Enable the bundle in your app's `Appkernel`:

```php
# app/AppKernel.php
class AppKernel extends Kernel
{
    public function registerBundles()
    {
        $bundles = array(
        	...
            new Dzango\Bundle\TwigTruncateBundle\TwigTruncateBundle(),
            ...
        );
```

Usage
-----

See the [TwigTruncateExtension](https://github.com/dzango/TwigTruncateExtension)'s documentation.

