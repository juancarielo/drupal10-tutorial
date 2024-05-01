[<img alt="Drupal Logo" src="https://www.drupal.org/files/Wordmark_blue_RGB.png" height="80px">](https://drupal.org)

Just a simple Drupal 10 project for tutorial.

## Requirements

Versions I'm currently using:

- [Docker](https://docs.docker.com/engine/install/) v20.10.22, build 3a2c30b
- [Docker Compose](https://docs.docker.com/engine/install/) v2.15.1
- [DDEV](https://ddev.readthedocs.io/en/latest/users/install/ddev-installation/) v1.22.7
- [Git](https://git-scm.com/downloads) v2.39.3

## Install

Clone the repo into a folder of your preference:
```sh
git clone git@github.com:juancarielo/drupal10-tutorial.git && cd drupal10-tutorial
```
Configure DDEV project (optional):
```sh
ddev config --project-type=drupal10 --docroot=web --create-docroot
```
Then start the project:
```sh
ddev start
```
Install dependencies using Composer:
```sh
ddev composer install
```
To stop:
```sh
ddev stop
```
To delete, execute this line:
```sh
ddev delete -Oy
```

---

## Tips

Create a project without installation, just generating the `composer.json` and `composer.lock` files:
```sh
composer create-project drupal/recommended-project . --no-install
```