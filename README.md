Yii2 RSS
========
Yii2 RSS Feeder and Reader

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist orezomi/yii2rss "*"
```

or add

```
"orezomi/yii2rss": "*"
```

to the require section of your `composer.json` file.

Usage
-----
Configuration web.php
```
'components' => [
       ...
    	'feed'=>[
    		'class'=>'orezomi\yii2rss\Feedoz',
    	],
    	...
    	]
```
and in controller or view use this to get feed:
```
$feed=Yii::$app->feed->reader()->import('http://example.com/rss');
```
