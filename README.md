# dockerfiles

Various Dockerfiles for images I created.

You should find these on dockerhub under [vguillou](https://hub.docker.com/u/vguillou/).

## Commands

Examples for `centos-node:7.7-10.16.3`.

```sh
cd centos-node/7.7-10.16.3/
```

#### Build an image

```sh
docker login -u {YOUR DOCKERHUB USERNAME}
docker build -t centos-node .
```

#### Tag an image

```sh
docker images # Find the IMAGE ID of the centos-node image
docker tag {IMAGE ID} vguillou/centos-node:7.7-10.16.3
```

#### Upload tagged image manually to dockerhub

*Note: Rather obviously, this will replace any previous image that had the same tag.*

```sh
docker push vguillou/centos-node:7.7-10.16.3
```