# Docker Setup for PHP 8.2
Docker setup for development with PHP 8.2 running under `:8082` port.

### Post Clone
You MUST create the directory `code` where you'll maintain your projects.
```bash
mkdir code
```
Docker maps your projects by creating a volume upon `code` directory.

### Setup Info
1. Image: [php:8.2-rc-apache-bullseye](https://hub.docker.com/layers/library/php/8.2-rc-apache-bullseye/images/sha256-cf436a6f11324235aba7f51f95be81a43cd9ca859423a4cae78e09bbd908d7b8?context=explore)
2. Available apps: `composer` v2.2, `vim`, `git`
3. You can edit Apache's default vhost in `docker/apache/000-default.conf`.
4. You can edit `php.ini` in `Dockerfile`.
5. Please replace my Github info with yours in `Dockerfile`.
6. The container will listen to `:8082` port, so you can access your projects on `http://localhost:8082/`

### Changing PHP version
Change the branch to change PHP version.
```bash
# Changing to PHP 8.2
git fetch && git checkout php-8.2
```