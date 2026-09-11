# Docker Deployment

## Nginx Container Deployment

### 1. Pull the Nginx Image

```bash
docker pull nginx
```

This command downloads the official Nginx image from Docker Hub.

### 2. Run the Nginx Container

```bash
docker run -d -p 8080:80 nginx
```

This command runs the Nginx container in the background and maps port 8080 on the host to port 80 inside the container.

### 3. Test the Nginx Web Server

```bash
curl http://localhost:8080
```

This command sends a request to the Nginx web server and displays its HTML welcome page.

The output showed "Welcome to nginx!", which confirmed that the web server was running successfully.

## Container Lifecycle

### 1. List Running Containers

```bash
docker ps
```

This command shows the Nginx container that is currently running.

### 2. Stop the Running Container

```bash
docker stop df906e73429c
```

This command stops the running Nginx container.

### 3. Verify It Is Stopped

```bash
docker ps -a
```

This command shows all containers and confirms that the Nginx container has stopped with an `Exited (0)` status.

### 4. Remove the Container Completely

```bash
docker rm df906e73429c
```

This command removes the stopped Nginx container completely.

## Result

The Nginx web server was successfully deployed using Docker and tested through port 8080. The container was then stopped, checked, and removed using basic Docker commands.
