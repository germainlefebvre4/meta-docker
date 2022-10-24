# Quick reference

* Maintained by: 
  [germainlefebvre4](https://github.com/germainlefebvre4)


# Supported tags and respective Dockerfile links

* [`18`](https://github.com/germainlefebvre4/meta-docker/blob/main/Dockerfile-node18), [`node18`](https://github.com/germainlefebvre4/meta-docker/blob/main/Dockerfile-node18), [`latest`](https://github.com/germainlefebvre4/meta-docker/blob/main/Dockerfile-node18)
* [`16`](https://github.com/germainlefebvre4/meta-docker/blob/main/Dockerfile-node16), [`node16`](https://github.com/germainlefebvre4/meta-docker/blob/main/Dockerfile-node16)


# Getting started

```bash
docker run --rm -v $(pwd):/app germainlefebvre4/meta:latest meta git update
```


# What is meta?

meta is a tool for managing multi-project systems and libraries. It answers the conundrum of choosing between a mono repo or many repos by saying "both", with a meta repo!

meta is powered by plugins that wrap common commands, letting you execute them against some or all of the repos in your solution at once. meta is built on loop, and as such inherits loops ability to easily target a particular set of directories for executing a common command (eg meta git status --include-only dir1,dir2. See loop for more available options).

meta is packaged with a few of these core plugins by default: https://github.com/mateodelnorte/meta/blob/master/package.json#L63-L66


[https://www.npmjs.com/package/meta](https://www.npmjs.com/package/meta)


# Dockerfile

```Dockerfile
FROM node:18

WORKDIR /app

RUN npm i -g meta
```

