docker-caddy-wordpress-mariadb
---

## Features
- One line command to setup your wordpress stack
- Enabling ssl by default thanks to Caddy
- Using mariadb for slightly better performace

## prepare
- docker, docker-compose: https://www.docker.com/get-started

## start up
1. copy `env.example` into `.env` with you own secret
```
cp env.example .env
vim .env
...
...
```
2. modify `Caddyfile`, replace localhost with your own domain (more configuration: https://caddyserver.com/docs/)
3. start with command `docker-compose-up`
```
docker-compose up
```

## credits
- https://blog.kernl.us/2019/10/wordpress-database-performance-showdown-mysql-vs-mariadb-vs-percona/
- https://minhcung.me/how-to-start-wordpress-with-caddy/
