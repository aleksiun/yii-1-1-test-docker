# yii-1-1-test-docker

Yii 1.1.20 Framework test app based on Docker

Based on "The Definitive Guide to Yii 1.0":

EN: https://www.yiiframework.com/doc/guide/1.1/en

PL: https://www.yiiframework.com/doc/guide/1.1/pl

Docker environment:

- php:5.6-apache
- mysql:5.7.35
- phpmyadmin:5.1.1
- memcached:latest

Locations:

- "testdrive/" - Yii test application folder
- "requirements/index.php" - Yii Requirement Checker - now Memcache extension = Failed
- "configs/php5-apache-dockerfile" - PHP Dockerfile
