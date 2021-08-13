# yii-1-1-test-docker

Yii 1.1.20 Framework test app based on Docker

Based on:

EN: https://www.yiiframework.com/doc/guide/1.1/en

PL: https://www.yiiframework.com/doc/guide/1.1/pl

Framework:

https://github.com/yiisoft/yii/releases/tag/1.1.20

Docker environment:

- php:5.6-apache
- mysql:5.7.35
- phpmyadmin:5.1.1
- memcached:latest

Locations:

- "application/testdrive/" - Yii test application folder
- "application/testdrive/protected/config/main.php" - Yii config file (inc. Gii config)
- "application/testdrive/protected/config/database.php" - Yii database config file
- "requirements/index.php" - Yii Requirement Checker - now Memcache extension = Failed
- "configs/php5-apache-dockerfile" - PHP Dockerfile

To do:

- Docker network fix (static IP for containers?)
- chmod fix (avoid "chmod -R 777 html")
- PHP 7, 8
- MySQL 8

Temp notes:

Gii permission fix (temporary)

chown -R www-data:www-data /var/www/html/testdrive

or

chmod -R 777 html
