# Jenkins Docker

Simple docker image to be able jenkins user to do sudo without password.

example how to run:

```
docker run -d \
  -v /var/run/docker.sock:/var/run/docker.sock \
  -v $(which docker):/usr/bin/docker \
  -p 8080:8080 \
  ryanhs/jenkins:lts-docker
```


> reference: [https://container-solutions.com/running-docker-in-jenkins-in-docker/](https://container-solutions.com/running-docker-in-jenkins-in-docker/)
