# Install
* Install Docker [mac](https://store.docker.com/editions/community/docker-ce-desktop-mac) | [windows](https://store.docker.com/editions/community/docker-ce-desktop-windows) | [linux](https://docs.docker.com/install/linux/docker-ce/ubuntu/)

# Config
* Copy `.env.dist`  →  `.env`
* Set path to website in .`env` → `WWW_PATH`

# Start
`docker-compose up`

# Commands
(3rd arg → container name (php, nginx etc...))
* `docker-compose exec php php /code/artisan`
