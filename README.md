# Python with Node env to run tests

Base image with:
- python 3.7.3
- node 10.15.3
- npm 6.9.0
- angular cli 7.3.9

# Docker hub

[dcmir/docker-python-gcloud-node](https://hub.docker.com/r/dcmir/docker-python-gcloud-node/)

# Commands


## Build the image
```
docker build -t dcmir/docker-python-gcloud-node:[vN] .
```

## Push the image

```
docker push dcmir/docker-python-gcloud-node:[vN]
```

## Test local

```
docker run -it --volume=<application_path>:/localDebugRepo --workdir="/localDebugRepo" --memory=4g --memory-swap=4g --memory-swappiness=0 --entrypoint=/bin/bash dcmir/docker-python-gcloud-node
```

vN -> Is the docker version
