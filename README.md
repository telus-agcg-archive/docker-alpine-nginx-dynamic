# Alpine Nginx Dynamic

Tiny web server using nginx built from source on Alpine Linux that supports dynamic upstream servers via [nginx-upstream-dynamic-servers](https://github.com/GUI/nginx-upstream-dyanmic-servers).

The current version of Nginx availble in apk is 1.6.2:

```sh
/ # apk --update search nginx
nginx-1.6.2-r1
```

This image builds the latest version (1.7.11) from source:

```sh
docker run -it --rm connexiolabs/alpine-nginx:1.7.11 sh

> nginx -v
nginx version: nginx/1.7.11
```

Built image currently weighs in at 28.1 MB:

```sh
❯ docker images | grep dynamic
connexiolabs/alpine-nginx-dynamic:latest  4c2eb132cfca  3 minutes ago  28.15 MB
```
