<p align="center">
    <a href="https://github.com/yiisoft" target="_blank">
        <img src="https://avatars0.githubusercontent.com/u/993323" height="100px">
    </a>
    <h1 align="center">Yii 2 Advanced Project Template</h1>
    <br>
</p>

Yii 2 Advanced Project Template is a skeleton [Yii 2](http://www.yiiframework.com/) application best for
developing complex Web applications with multiple tiers.

The template includes three tiers: front end, back end, and console, each of which
is a separate Yii application.

The template is designed to work in a team development environment. It supports
deploying the application in different environments.

The first steps
-------------------
1. Configure the database connection in the config:
```
/common/config/main-local.php
```
2. Configure the test database connection in the config:
```
/common/config/test-local.php
```
3. Create directory for database dump:
```
mkdir console/migrations-tests
```
4. Create database dump:
```
php yii migrate

php yii migrate/dump

mysql -uroot -proot yii2advanced_test < console/migrations-tests/dump.sql
```