# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

This mission focused on deploying a multi-tier application using Docker Compose. We created a Nextcloud application container and a MariaDB database container. We also learned how the two containers work together.

## Objectives

* Understand multi-tier architecture
* Create a Docker Compose configuration
* Deploy Nextcloud and MariaDB containers
* Connect the application container to the database container
* Practice starting and stopping multiple containers
* Document the deployment process

## Commands Executed

```bash
docker-compose --version
docker-compose config
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

In this activity, I learned how to use Docker Compose to manage multiple containers. I learned how Nextcloud connects to MariaDB using the `MYSQL_HOST` setting. I also learned the difference between running one container with `docker run` and managing multiple containers with `docker-compose up -d`. This activity also helped me practice checking container status and documenting the deployment process.
