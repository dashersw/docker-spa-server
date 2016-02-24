# Tiny single page application server for Docker

This is a very small docker image based on [Node.js on Alpine Linux](https://github.com/mhart/alpine-node).

It runs a fork of [http-server](https://github.com/indexzero/http-server) and expects a volume to be mounted as the /app folder. The image listens on port 8080 by default.

Running this image would look like:
```
docker run -it -v /data/single-page-app:/app -p 8080:8080 dashersw/spa-server
```
