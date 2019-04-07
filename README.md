# daroachtech

> a dream for the future

here you can find the workings of my [network stack](https://www.instagram.com/p/BtSgNa8ni0i/?utm_source=ig_web_button_share_sheet). I have example docker compose files for all my major web services, compartmentalized into folder groups.

## dtech_engine

this is my implementation of the core of my server stack. this docker-compose file spins up jwilder's [nginx proxy](https://hub.docker.com/r/jwilder/nginx-proxy/) container and the popular letencrypt [proxy companion](https://hub.docker.com/r/jrcs/letsencrypt-nginx-proxy-companion/) container.

## daroach.net

A work in progress personal page. Here, I hope to start a blog detailing the new things I am learning how to do with a computer. This container spins up a nginx server that serves the content on my servers `/srv/webroot` directory. Example docker-compose file working with jwilder's proxy tool.

* I want to re-write this in vue.js

[about me](daroach.net/about)

## dtech_cloud
> cloud.daroach.net

[`nextcloud:fpm`](https://github.com/nextcloud/docker/blob/master/.examples/docker-compose/with-nginx-proxy/mariadb-cron-redis/fpm/docker-compose.yml) implementation.

## dtech_dynamic_dns

docker-compose file that initalizes my google dynamic dns pinging agents. ping every 42 mins to update my consumer grade spectrum internet non-static ip address. i use google domains to handle my nameservers and url addresses.

## my initialization steps

### how i start my servers

1. start google dyanmic dns services.
2. start my daroachtech engine
3. start whatever services i want from there.

### to start a docker-compose file

1. `docker-compose build --pull`
2. `docker-compose up -d`
3. `docker-compose logs -f`

~~``` internal look only, if you are seeing this please look away ```~~
**UPDATE** As of March 25, 2019 this repository is public.
