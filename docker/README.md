##### Docker Images
- Node: https://github.com/nodejs/docker-node
- Usage:
```
FROM node:4-onbuild
# replace this with your application's default port
EXPOSE 8888
```
- Running:
```shell
$ docker build -t my-nodejs-app .
$ docker run -it --rm --name my-running-app my-nodejs-app
```