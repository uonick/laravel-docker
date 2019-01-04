![Header](https://i.imgur.com/RGvYEaS.png)

# Intro
This repo contains the source of PHP development environment for Docker.

* Ubuntu 18.04
* MySQL 8.x
* PHP 7.3.x
* Redis 5.0.x
* Docker compose file

## Install
* Install Docker [macOS](https://store.docker.com/editions/community/docker-ce-desktop-mac) | [Linux](https://docs.docker.com/install/linux/docker-ce/ubuntu/) | [Windows](https://store.docker.com/editions/community/docker-ce-desktop-windows)

## Config
* Copy `.env.dist`  →  `.env`
* Set path to website in `.env` → `WWW_PATH`

## Start
* `docker-compose up`

## MySQL
* MySQL host: `mysql` (`127.0.0.1` from host)
* MySQL user: `laravel`
* MySQL password: `laravel`

and

* MySQL root user: `root`
* MySQL root password: `root`

## Commands
* Show images `docker ps`
* Execute command`docker-compose exec php php /code/artisan`
(3rd arg → container name (php, nginx etc...))

# Default directories
* Sources: `./www/` → `/code`
* Database: `./database`
* Logs: `./docker/logs/mysql`, `./docker/logs/nginx`

![screenshot](www/public/screenshot.png)
