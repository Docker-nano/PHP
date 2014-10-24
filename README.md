Nano PHP with Composer
======================

[![Build status][Build image]][Build]

This is the [Docker Nano](https://github.com/Docker-nano) image for [PHP](http://php.net) v5.5.16 with
[Composer](http://getcomposer.org).

* Docker Hub image: [`nano/php-composer`][Docker Hub repo]
* Size: ~9MB

Usage
-----

Try one of the following.

* Run PHP with `docker run -it nano/php-composer:latest`
* Run Composer with `docker run -it nano/php-composer:latest composer`
* Add `FROM nano/php-composer:latest` to your Dockerfile.

  [Build]: http://travis-ci.org/Docker-nano/PHP
  [Build image]: http://img.shields.io/travis/Docker-nano/PHP.svg "Build status"
  [Docker Hub repo]: https://registry.hub.docker.com/u/nano/php-composer/
