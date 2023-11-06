# Dockerization of Node.js Application

Here we are doing the following:

- Pulling Ubuntu Base Image.
- Updating & Installing Node.js.
- Copying Files from Local to Docker Container.
- Installing NPM Packages.
- Running Express Server.

Get this Image (nirmalya1998/node-docker) from Docker Hub [here](https://hub.docker.com/r/nirmalya1998/node-docker).

## Available Commands

| command                                                                               | description                                                    |
| :------------------------------------------------------------------------------------ | :------------------------------------------------------------- |
| `docker build -t node-docker .`                                                       | Build Image from current directory                             |
| `docker run -it -v D:\Code\docker-node:/home/node-docker --name nirmalya node-docker` | Mount Drive & Run Interactively                                |
| `docker run -it -e PORT=8080 -p 8080:8080 docker-node`                                | Start app with port forwarded & environment variable mentioned |
| `docker exec -it serene_easley bash`                                                  | Run 'bash' Interactively                                       |
