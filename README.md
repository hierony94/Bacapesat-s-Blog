# Bacapesat-s-Blog

## Introduction
This Bacapesat blog using Dockerized Ghost + Letsencrypt nginx proxy companion

You can see the detail for each in:
 - Ghost, https://hub.docker.com/_/ghost/

 - Letsencrypt nginx proxy companion, https://hub.docker.com/r/jrcs/letsencrypt-nginx-proxy-companion/
 
 
## Requirement
- Docker : [http://docs.docker.com/installation/](http://docs.docker.com/installation/)

- docker-compose : [https://github.com/docker/compose/releases](https://github.com/docker/compose/releases)

## Run Instructions
1. Move to proxy folder by run `cd proxy` and then run letsencrypt nginx proxy container using docker-compose
```bash
docker-compose build && docker-compose up -d
```

2. Move to app folder by run `cd app` and then run the ghost app container using docker-compose
```bash
docker-compose build && docker-compose up -d
```

3. Finish

## Notes

Make sure you edit docker-compose of app (https://github.com/HieronyM/Bacapesat-s-Blog/blob/master/app/docker-compose.yml) and change the **VIRTUAL_HOST**, **LETSENCRYPT_HOST** with your blog url. and change **LETSENCRYPT_EMAIL** with your email
