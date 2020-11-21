# jenkins-docker
Jenkins with Docker installed inside a docker container for CICD

## Running jenkins with docker from host:

1. To run the container, you need to add a volume in docker run command:

```
… -v /var/run/docker.sock:/var/run/docker.sock …
```

2. The complete run command:

```
 docker run --name jenkins-docker -p 8080:8080 -v /var/run/docker.sock:/var/run/docker.sock jenkins-docker
```

