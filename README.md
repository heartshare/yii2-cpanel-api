Yii2 cPanel API
===============
Yii2 extension for cpanel/whm

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist poshtiban/yii2-cpanel-api "*"
```

or add

```
"poshtiban/yii2-cpanel-api": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply use it in your code by  :

```php
<?
    $cpanel = new \poshtiban\cpanelAPI\cPanel([
        'host'=>'localhost',
        'port'=>'2083',
        'username'=>'demo',
        'password'=>'demo',
    ]); 
    $cpanel->addSubdomain([
        'name'=>'subdemo',
        'domain'=>'example.com',
    ]);

?>```