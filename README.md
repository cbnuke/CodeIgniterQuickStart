# CodeIgniter Quick Start
CodeIgniter Quick Start is combination any required for develop website
based on CodeIgniter version 3.0 .

## Folder Structure

```
CodeIgniterQuickStart/
├── application/
    └── config/
    └── controllers/
    └── models/
    └── views/
    └── ...
├── assets/
    └── css/
    └── img/
    └── js/
    └── ...
├── .htaccess
├── composer.json
├── composer.lock
├── index.php
└── vendor/
    └── codeigniter/
    └── ...
```

* If you're structure don't like this. You haven't update package with `Composer`.

## Requirements

* PHP 5.4 or newer is recommended
* Composer for get/update any package require (See [Composer Installation](https://getcomposer.org/doc/00-intro.md))
* Git for update CodeIgniter Quick Start

## How to Use

### Clone This repository
Many way to clone such as github WebUI `Clone in Desktop` or `Download ZIP`

### Update any package with Composer
Go to root folder CodeIgniterQuickStart and run this command

```
$ composer update
```

### Success
Now you can develop website by CodeIgniter pattern.
All your code are in folder `application` and static files in `assets`

## Simple develop by Codeigniter

### Change configuration
And it changes `application/config/config.php`:

~~~
$config['base_url'] = 'http://localhost/AccKK/';
↓
$config['base_url'] = 'YOUR SITE LOCATION';
~~~


#### How to use Asset Helper
Asset Helper are available to access static assets in folder `assets`
such as images, css, java script, etc.

```
├── assets/
    └── css/
    └── download/
    └── fonts/
    └── img/
    └── js/
    └── less/
    └── swf/
    └── upload/
    └── xml/
```

And you can call function to use auto style static assets.

~~~
<?=img('test.jpg')?>
<?=css('style.css')?>
<?=less('style.less')?>
<?=js('bootstrap.min.js')?>
...
~~~

Or you can call function to use URL paths.

~~~
<?=img_url()?>test.jpg
<?=css_url()?>style.css
<?=less_url()?>style.less
<?=js_url()?>bootstrap.min.js
...
~~~

* Document Asset Helper ([See more](https://github.com/sekati/codeigniter-asset-helper))

## Related Projects

* [CodeIgniter](https://github.com/bcit-ci/CodeIgniter)
* [Asset Helper Spark for CodeIgniter(sekati)](https://github.com/sekati/codeigniter-asset-helper)
