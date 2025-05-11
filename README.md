# Docker Compose Catalog 

This repository is what I use to version the stacks that I use most for studying and testing.

## Script Docker Clear

With this script you can clean your entire Docker

```bash
docker container rm -f $(docker container ls -qa)
docker image rm -f $(docker image ls -q)
docker network rm -f $(docker network ls -q)
docker volume rm -f $(docker volume ls -q)
docker system prune --all --force
```