# meta-docker

## Getting started

```bash
docker run --rm -v $(pwd):/app germainlefebvre4/meta:latest meta git update
```


## Build the docker images

```bash
NODE_VERSION=18

docker build -t germainlefebvre4/meta:node${NODE_VERSION} -t germainlefebvre4/meta:${NODE_VERSION} .
# docker build -t germainlefebvre4/meta:latest .

docker push germainlefebvre4/meta:node${NODE_VERSION}
docker push germainlefebvre4/meta:${NODE_VERSION}
# #docker push germainlefebvre4/meta:latest
```
