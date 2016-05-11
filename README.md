# Let's Encrypt Dockerfile

[![Docker Pulls](https://img.shields.io/docker/pulls/almeida/letsencrypt.svg)](https://hub.docker.com/r/almeida/letsencrypt/)
[![Docker Stars](https://img.shields.io/docker/stars/almeida/letsencrypt.svg)](https://hub.docker.com/r/almeida/letsencrypt/)

## Description

Let's Encrypt client.

### Volumes

 * /etc/letsencrypt
 * /var/lib/letsencrypt
 * /var/www/acme-challenge

## Run

	$ docker run -d \
		--name letsencrypt \
		-v /somehostdir/letsencrypt/etc/:/etc/letsencrypt/ \
		-v /somehostdir/letsencrypt/var/:/var/lib/letsencrypt/ \
		-v /somehostdir/letsencrypt/www/:/var/www/acme-challenge/ \		
		almeida/letsencrypt
