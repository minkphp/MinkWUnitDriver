Mink WUnit Driver
=================

Usage Example
-------------

``` php
<?php

use Behat\Mink\Mink,
    Behat\Mink\Session,
    Behat\Mink\Driver\WUnitDriver;

$mink = new Mink(array(
    'wunit' => new Session(new WUnitDriver()),
));

$mink->getSession('wunit')->getPage()->findLink('Chat')->click();
```

Installation
------------

``` json
{
    "requires": {
        "behat/mink":              "1.4.*",
        "behat/mink-wunit-driver": "*"
    }
}
```

``` bash
curl http://getcomposer.org/installer | php
php composer.phar install
```

Copyright
---------

Copyright (c) 2012 Patrick Dreyer (patrick.dreyer.name). See LICENSE for details.

Maintainers
-----------

* Patrick Dreyer [patrickdreyer](http://github.com/patrickdreyer)
