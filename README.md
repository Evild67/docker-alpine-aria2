[![Docker Stars](https://img.shields.io/docker/stars/evild/alpine-aria2.svg?style=flat-square)](https://hub.docker.com/r/evild/alpine-aria2/)
[![Docker Pulls](https://img.shields.io/docker/pulls/evild/alpine-aria2.svg?style=flat-square)](https://hub.docker.com/r/evild/alpine-aria2/)
[![ImageLayers Size](https://img.shields.io/imagelayers/image-size/evild/alpine-aria2/latest.svg?style=flat-square)](https://hub.docker.com/r/evild/alpine-aria2/)

# Alpine Aria2

This image is based on [evild/alpine-base](https://hub.docker.com/r/evild/alpine-base/)

## Version

### Stable

- `stable`, `latest` [(Dockerfile)](https://github.com/Evild67/docker-alpine-aria2/blob/master/Dockerfile)
- `1.22.0` [(Dockerfile)](https://github.com/Evild67/docker-alpine-aria2/blob/master/90c51b1365e6fb2049c873757e2503e848664c93/Dockerfile)

## What is aria2?
aria2 is a utility for downloading files. The supported protocols are HTTP(S), FTP, SFTP, BitTorrent, and Metalink. aria2 can download a file from multiple sources/protocols and tries to utilize your maximum download bandwidth. It supports downloading a file from HTTP(S)/FTP/SFTP and BitTorrent at the same time, while the data downloaded from HTTP(S)/FTP/SFTP is uploaded to the BitTorrent swarm. Using Metalink's chunk checksums, aria2 automatically validates chunks of data while downloading a file like BitTorrent.

## Installation
Automated builds of the image are available on Dockerhub and is the recommended method of installation.
```
docker pull evild/alpine-aria2:1.22.0
```

You can also pull the latest tag which is built from the repository HEAD : aria2 Mainline with Openssl.
```
docker pull evild/alpine-aria2:latest
```


## Basic usage
```docker run -p 6800:6800 -e ARIA2_SECRET_TOKEN=mysecretoken --name aria2 evild/alpine-aria2```
