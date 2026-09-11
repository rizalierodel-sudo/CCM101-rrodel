# Laboratory 04 - Cloud-Native Engineer

## Mission Overview

In this laboratory activity, I learned how containers are used in cloud computing. I compared Virtual Machines and Containers and used the KillerCoda Playground to practice Docker commands. I also deployed an Nginx web server using Docker and managed its container through different lifecycle commands.

## Objectives

- Differentiate Virtual Machines from Containers.
- Access a Docker-enabled environment using KillerCoda.
- Execute basic Docker CLI commands.
- Pull and run an Nginx container.
- Test a containerized web server.
- Stop, verify, and remove a Docker container.
- Document Docker operations using Markdown.

## Docker Commands Executed

### Checkpoint 3 - Docker Playground

```bash
docker --version
```

Checks the installed Docker version.

```bash
docker info
```

Shows information about the Docker environment.

### Checkpoint 4 - Nginx Deployment

```bash
docker pull nginx
```

Downloads the official Nginx image from Docker Hub.

```bash
docker run -d -p 8080:80 nginx
```

Runs the Nginx container in detached mode and maps port 8080 to port 80.

```bash
docker ps
```

Lists the currently running containers.

```bash
curl http://localhost:8080
```

Tests the Nginx web server through port 8080.

### Checkpoint 5 - Container Lifecycle

```bash
docker ps
```

Lists the running containers.

```bash
docker stop df906e73429c
```

Stops the running Nginx container.

```bash
docker ps -a
```

Shows all containers and verifies that the Nginx container has stopped.

```bash
docker rm df906e73429c
```

Removes the stopped Nginx container.

```bash
docker ps -a
```

Checks that the removed container is no longer listed.

## Skills Learned

I learned how to use basic Docker commands and how to manage a container from starting it until removing it. I also learned how to deploy an Nginx web server and test it using the `curl` command. Most importantly, I became more familiar with using the terminal and documenting technical activities using Markdown.

## Challenges Encountered

One challenge I encountered was reconnecting to KillerCoda and having to start the Docker activity again. I also had to make sure that I was using the correct container ID when stopping and removing the Nginx container. After repeating the steps, I was able to successfully run, stop, and remove the container.
