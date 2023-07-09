# Docker Setup for PHP 8.1
Docker setup for development with PHP 8.1 runnig under `:8081` port.

### Post Clone
You MUST create the directory `code` where you'll maintain your projects.
```bash
mkdir code
```
Docker maps your projects by creating a volume upon `code` directory.

### Setup Info
1. Image: [php:8.1-apache-bullseye](https://hub.docker.com/layers/library/php/8.1-apache-bullseye/images/sha256-3d51d2ab08496667ec310e82c205ba03c3b8bf9a950447d257b66639cd9e194e?context=explore)'
2. Available apps: `composer` v2.2, `vim`, `git`
3. You can edit Apache's default vhost in `docker/apache/000-default.conf`.
4. You can edit `php.ini` in `Dockerfile`.
5. Please replace my Github info with yours in `Dockerfile`.
6. The container will listen to `:8081` port, so you can access your projects on `http://localhost:8081/`

### Changing PHP version
Change the branch to change PHP version.
```bash
# Changing to PHP 7.1
git fetch && git checkout php-7.1
```
