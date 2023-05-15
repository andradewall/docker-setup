# Docker Setup for PHP 7.1
Docker setup for development with PHP 7.1 runnig under `:8071` port.

### Post Clone
You MUST create the directory `code` where you'll maintain your projects.
```bash
mkdir code
```
Docker maps your projects by creating a volume upon `code` directory.

### Setup Info
1. Image: [php:7.1-apache-stretch](https://hub.docker.com/layers/library/php/7.1-apache-stretch/images/sha256-d6ce146ca4d868023314a29f799fbfabbdb483c1db598ed5c935b047c830da7a?context=explore)
2. Available apps: [`composer`, `vim`, `git`]
3. You can edit Apache's default vhost in `docker/apache/000-default.conf`.
4. You can edit `php.ini` in `Dockerfile`.
5. Please replace my Github info with yours in `Dockerfile`.
6. The container will listen to `:8071` port, so you can access your projects on `http://localhost:8071/`

### Changing PHP version
Change the branch to change PHP version.
```bash
# Changing to PHP 8.2
git fetch && git checkout php-8.2
```