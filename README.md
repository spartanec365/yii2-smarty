Smarty Extension for Yii 2
==========================

This extension provides a `ViewRender` that would allow you to use [Smarty](http://www.smarty.net/) view template engine.

For license information check the [LICENSE](LICENSE.md)-file.

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist yiisoft/yii2-smarty
```

or add

```json
"yiisoft/yii2-smarty": "~2.0.0"
```

to the require section of your composer.json.

Note that the smarty composer package is distributed using subversion so you may need to install subversion.

Usage
-----

To use this extension, simply add the following code in your application configuration:

```php
return [
    //....
    'components' => [
        'view' => [
            'renderers' => [
                'tpl' => [
                    'class' => 'yii\smarty\ViewRenderer',
                    //'cachePath' => '@runtime/Smarty/cache',
                ],
            ],
        ],
    ],
];
```
