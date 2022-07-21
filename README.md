# docker-containers
CI/CD Docker Containers



```shell
docker build -t backstopjs-node:14 -f backstopjs-node/14/Dockerfile .
docker build -t backstopjs-node:16 -f backstopjs-node/16/Dockerfile .
docker build -t backstopjs-node:18 -f backstopjs-node/18/Dockerfile .

# check node versions
docker run -it  -t backstopjs-node:14 node -v
docker run -it  -t backstopjs-node:16 node -v
docker run -it  -t backstopjs-node:18 node -v

docker image tag backstopjs-node:14 klodoma/backstopjs-node:14
docker image tag backstopjs-node:16 klodoma/backstopjs-node:16
docker image tag backstopjs-node:18 klodoma/backstopjs-node:18

docker push klodoma/backstopjs-node:14
docker push klodoma/backstopjs-node:16
docker push klodoma/backstopjs-node:18
```
