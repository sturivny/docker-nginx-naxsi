[![Docker Stars](https://img.shields.io/docker/stars/dmgnx/nginx-naxsi.svg)](https://hub.docker.com/r/dmgnx/nginx-naxsi/)
[![Docker Pulls](https://img.shields.io/docker/pulls/dmgnx/nginx-naxsi.svg)](https://hub.docker.com/r/dmgnx/nginx-naxsi/)
[![Docker Automated buil](https://img.shields.io/docker/automated/dmgnx/nginx-naxsi.svg)](https://hub.docker.com/r/dmgnx/nginx-naxsi/)

# Supported tags and respective `Dockerfile` links

-   [`1.17.3-0.56`, `mainline`, `latest` (*mainline/Dockerfile*)](https://github.com/dmgnx/docker-nginx-naxsi/blob/master/mainline/Dockerfile)
-   [`1.16.1-0.56`, `stable` (*stable/Dockerfile*)](https://github.com/dmgnx/docker-nginx-naxsi/blob/master/stable/Dockerfile)

# How to use this image

```console
$ docker run --name nginx-naxsi -p 80:80 \
    -v $(pwd):/usr/share/nginx/html -d dmgnx/nginx-naxsi
```

This will start a nginx service with default configuration, serving current working directory as your website.

# Volumes

-   `/etc/nginx/conf.d` : virtual hosts configuration
-   `/etc/nginx/naxsi` : your Naxsi rules
-   `/etc/nginx/ssl` : SSL certificates
-   `/usr/share/nginx/html` : web root directory
-   `/var/log/nginx` : log storage (redirected to the standard outputs by default)
