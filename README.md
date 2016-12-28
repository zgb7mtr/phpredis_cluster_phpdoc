# phpredis_cluster_phpdoc

You need to add the path to a class of global include path.

After that, your IDE, when you declare a class Redis will display a hint which methods of this object can be used.

### For example:

    $redisCluster = new RedisCluster(null,['127.0.0.1:6379']);
    $redisCluster->se<press Tab or press Ctrl+Space>

### Install

 * Install [redis-server](http://redis.io/download)
 * Install [phpredis extension](https://github.com/nicolasff/phpredis)
 * The simpliest way to install and use phpredis_cluster_phpdoc is to use Composer, as there is a [package on Packagist](https://packagist.org/packages/zgb7mtr/phpredis_cluster_phpdoc). Just add this to your project composer.json file :

        {    
        "require": {        
            "zgb7mtr/phpredis_cluster_phpdoc": "*"
        },        
        "minimum-stability": "dev"        
        }

 * Or direct download [phpredis_cluster_phpdoc](https://github.com/zgb7mtr/phpredis_cluster_phpdoc/tarball/master)

### Setup in IDE PhpStorm

 Menu "File" -> "Settings" -> "Languages & Frameworks" ->  "PHP" -> "Include Path" ->  _Select path to folder "phpredis_cluster_phpdoc"_

### Setup in IDE NetBeans

 * Right click your project -> "Properties"
 * Select the "PHP Include Path" category
 * Click "Add Folder..."
 * Select your checkout of phpredis_cluster_phpdoc
 * Click "Open"
 * Click "OK"

### Setup in Zend Studio IDE (Eclipse PDT)

 * Open "Window" -> "Preferences"
 * In preferences dialog open "PHP" -> "PHP Libriaries"
 * Click "New" button, in "User library name" enter "Redis", click "OK"
 * Select newly created "Redis", library Click "Add external folder", select path to the folder which contains your checkout of phpredis_cluster_phpdoc or you can download single "RedisCluster.php" file https://raw.github.com/zgb7mtr/phpredis_cluster_phpdoc/master/src/RedisCluster.php
 * Include your custom library in your project: open "Project" -> "Properties" -> "PHP Include Path", click add library, select "User library", click "Next", check "Redis", click "Finish"
