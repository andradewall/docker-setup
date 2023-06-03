# Docker Setup for PHP 7.3
Docker setup for development with PHP 7.3 runnig under `:8073` port.

### Post Clone
You MUST create the directory `code` where you'll maintain your projects.
```bash
mkdir code
```
Docker maps your projects by creating a volume upon `code` directory.

### Setup Info
1. Image: [php:7.3-apache-stretch](https://hub.docker.com/layers/library/php/7.3-apache-stretch/images/sha256-78605f6e1e833d5bf397bc8fb249becf9d86469477d3679124fd2134749b6761?context=explore)
2. Available apps: `composer` v2.2, `vim`, `git`
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