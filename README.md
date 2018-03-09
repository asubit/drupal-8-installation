# Drupal 8 quick installation guide

## Useful docs

- [Drupal 8 Documentation.](https://www.drupal.org/docs/8)
- [Drupal 8 User Guide](https://www.drupal.org/docs/user_guide/en/index.html)
- [Drupal 8 User Guide - Chapter 3. Installation](https://www.drupal.org/docs/user_guide/en/installation-chapter.html)
- [Drupal 8 User Guide - Chapter 3.1. Concept: Server Requirements](https://www.drupal.org/docs/user_guide/en/install-requirements.html)

## Before installation

### AMP stack

- Apache (or another web server)
- MySQL (or another database server)
- PHP

## Installation

### with Web installer

#### Download Drupal 8 core and other dev tools needed
- [Core](https://www.drupal.org/download)
- [Drupal 8 User Guide - Chapter 3.2. Concept: Additional Tools](https://www.drupal.org/docs/user_guide/en/install-tools.html)
- [Drush](http://www.drush.org/)
- [Git](https://git-scm.com/)
- [Composer](https://getcomposer.org/)
- [Devel](https://www.drupal.org/project/devel)
- [Drupal Console](https://drupalconsole.com/)
- [Coder](https://www.drupal.org/project/coder)

#### Run the web installer
- [Drupal 8 User Guide - Chapter 3.4. Running the installer](https://www.drupal.org/docs/user_guide/en/install-run.html)

### with Composer
- [Drupal.org - Using Composer to manage Drupal site dependencies](https://www.drupal.org/docs/develop/using-composer/using-composer-to-manage-drupal-site-dependencies)
- [Composer.org - Download](https://getcomposer.org/download/)
- [Composer.org - Documentation](https://getcomposer.org/doc/00-intro.md)

```
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('SHA384', 'composer-setup.php') === '544e09ee996cdf60ece3804abc52599c22b1f40f4323403c44d44fdfdd586475ca9813a858088ffbc1f233e9b180f061') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"

mv composer.phar /usr/local/bin/composer

composer create-project drupal/drupal my_site_name_dir

composer require drupal/<modulename>
```

## Dependencies
- [Install dependencies with composer](https://www.drupal.org/docs/8/install/step-2-install-dependencies-with-composer)

## Database
- [Create a Drupal database](https://www.drupal.org/docs/8/install/step-3-create-a-database)

## Configuration
- [Configure your installation](https://www.drupal.org/docs/8/install/step-4-configure-your-installation)

## Run installer
- [Run the installer](https://www.drupal.org/docs/8/install/step-5-run-the-installer)

## Status check
- [Status check](https://www.drupal.org/docs/8/install/step-6-status-check)

## [→ Drupal 8 quick dev guide](dev-guide)
