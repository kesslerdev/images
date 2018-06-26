# Docker client

compose example

```yml
version: '2'
services:
  docker-client:
    privileged: true
    image: kesslerdev/docker-client:latest
    stdin_open: true
    volumes:
    - /var/run/docker.sock:/var/run/docker.sock
    tty: true
    user: root
    labels:
      io.rancher.container.pull_image: always
      io.rancher.scheduler.global: 'true'
```
