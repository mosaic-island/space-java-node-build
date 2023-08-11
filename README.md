# Space Base JDK & Node Image
A customised OpenJDK base Docker image for JDK 17. This is to used for building Java/Node applications in Space.

## Build

To build the JDK 17 image and publish to Docker Hub

Ensure you have logged in to Docker Hub 

```shell
  docker login 
```

```shell
  docker buildx create --use
```

```shell
docker buildx build --push --platform linux/arm64/v8,linux/amd64 --tag miapplicationengineering/corretto-node-alpine:17.0.8 -f ./Dockerfile .
```

