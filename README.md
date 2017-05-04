# Drupalstack
Docker Compose based boilerplate for Drupal 8 development environment

## Featuring
* Apache 2.4
* PHP 7.1
* MariaDB 5.5
* Composer based Drupal installation 
* Drush
* Drupal Console
* PHPMyAdmin
* MailHog
## Installing Drupal
You should use Composer to install Drupal and all it's dependencies. Default dependencies, including Drupal core, are defined in ```web/composer.json``` which you can manage using ```$ docker-compose run composer <command>```. 
```bash
$ docker-compose run composer install
```
## Interacting with your installation
### Using Composer
```bash
$ docker-compose run composer <command>
```
### Using Drush
```bash
$ docker-compose run drush <command>
```
### Using Drupal Console
```bash
$ docker-compose run drupal <command>
```
### Console access to your Apache/PHP conatiner
```bash
$ docker exec -it <projectname>_web_1 bash
```
You have multiple containers running in your environment. Use ```drupal-compose ps``` to list all the containers you can connect to. 
