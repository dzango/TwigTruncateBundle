TwigTruncateBundle
==================

A Symfony bundle to include the [TwigTruncateExtension](https://github.com/dzango/TwigTruncateExtension) into your app. The TwigTruncateExtension allows you to truncate text while preserving HTML tags.

Installation
------------

Add the bundle to your app's `composer.json`:

```json
    "require": {
        "dzango/twig-truncate-bundle": "^1.0",
        ...
    }
```

Enable the bundle in your app's `Appkernel`(Only for symfony projects below 4):

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

Note:
In symfony 4 the bundle will automatically enabled in your app. In case the bundle does not enabled, add it to bundle list.  
```php
#config/bundles.php
return [
    ...
    Dzango\Bundle\TwigTruncateBundle\TwigTruncateBundle::class => ['all' => true],
]
```

Usage
-----

See the [TwigTruncateExtension](https://github.com/dzango/TwigTruncateExtension)'s documentation.

