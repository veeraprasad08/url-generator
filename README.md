The Puli URL Generator Component
================================

[![Build Status](https://travis-ci.org/puli/url-generator.svg?branch=master)](https://travis-ci.org/puli/url-generator)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/puli/url-generator/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/puli/url-generator/?branch=master)
[![SensioLabsInsight](https://insight.sensiolabs.com/projects/2197ba95-f3a5-4434-a11f-0ea4e37a74de/mini.png)](https://insight.sensiolabs.com/projects/2197ba95-f3a5-4434-a11f-0ea4e37a74de)
[![Latest Stable Version](https://poser.pugx.org/puli/url-generator/v/stable.svg)](https://packagist.org/packages/puli/url-generator)
[![Total Downloads](https://poser.pugx.org/puli/url-generator/downloads.svg)](https://packagist.org/packages/puli/url-generator)
[![Dependency Status](https://www.versioneye.com/php/puli:url-generator/1.0.0/badge.svg)](https://www.versioneye.com/php/puli:url-generator/1.0.0)

Latest release: none

PHP >= 5.3.9

The [Puli] URL Generator Component provides an API for generating URLs for Puli 
resources:

```php
echo $generator->generateUrl('/acme/blog/public/css/style.css');
```

The [UrlGenerator] can be created through the factory generated by the [Puli CLI]:

```php
$factoryClass = PULI_FACTORY_CLASS;
$factory = new $factoryClass();

$repo = $factory->createRepository();
$discovery = $factory->createDiscovery($repo);

$generator = $factory->createUrlGenerator($discovery);
```

Authors
-------

* [Bernhard Schussek] a.k.a. [@webmozart]
* [The Community Contributors]

Contribute
----------

Contributions to are very welcome!

* Report any bugs or issues you find on the [issue tracker].
* You can grab the source code at Puli’s [Git repository].

Support
-------

If you are having problems, send a mail to bschussek@gmail.com or shout out to
[@webmozart] on Twitter.

License
-------

All contents of this package are licensed under the [MIT license].

[Puli]: http://puli.io
[Bernhard Schussek]: http://webmozarts.com
[The Community Contributors]: https://github.com/puli/url-generator/graphs/contributors
[Getting Started]: http://docs.puli.io/en/latest/getting-started.html
[Puli Documentation]: http://docs.puli.io/en/latest/index.html
[issue tracker]: https://github.com/puli/issues/issues
[Git repository]: https://github.com/puli/url-generator
[Puli CLI]: https://github.com/puli/cli
[@webmozart]: https://twitter.com/webmozart
[MIT license]: LICENSE
[UrlGenerator]: http://api.puli.io/latest/class-Puli.UrlGenerator.Api.UrlGenerator.html
