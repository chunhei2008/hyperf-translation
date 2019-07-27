# Hyperf Translation


## Install

```
composer require chunhei2008/hyperf-translation

```

## Config


### publish config
```
php bin/hyperf.php  vendor:publish chunhei2008/hyperf-translation

```

### config path

```
your/config/path/autoload/translation.php

```

### config content

```
<?php

declare(strict_types=1);

/**
 * This file is part of Hyperf.
 *
 * @link     https://www.hyperf.io
 * @document https://doc.hyperf.io
 * @contact  group@hyperf.io
 * @license  https://github.com/hyperf-cloud/hyperf/blob/master/LICENSE
 */

return [
    'locale'          => 'en',   
    'fallback_locale' => '',
    'lang'            => BASE_PATH . '/resources/lang', 
];

```

## Usage


```

$translator = $this->container->get(\Chunhei2008\Hyperf\Translation\Contracts\Translator::class);

$translator->trans('validation.accepted'),
        

```