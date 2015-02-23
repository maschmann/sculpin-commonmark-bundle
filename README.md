# Sculpin CommonMark Bundle

[Sculpin](http://sculpin.io) bundle that integrates the [league/commonmark](https://github.com/thephpleague/commonmark) markdown parser.

## Installation

* Add the following to your `sculpin.json` file:

```json
{
    "require": {
        "bcremer/sculpin-commonmark-bundle": "dev-master"
    }
}
```

* Run `sculpin update`.
* Add the bundle to your kernel `app/SculpinKernel.php`:

```php
<?php

class SculpinKernel extends \Sculpin\Bundle\SculpinBundle\HttpKernel\AbstractKernel
{
    protected function getAdditionalSculpinBundles()
    {
        return array(
            'Bcremer\Sculpin\Bundle\CommonMarkBundle\SculpinCommonMarkBundle'
        );
    }
}
```

## License

The MIT License (MIT). Please see [License File](LICENSE) for more information.