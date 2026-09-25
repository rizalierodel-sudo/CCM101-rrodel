# Docker Compose Guide

## What does the services: block do?

The `services:` block defines the containers that will be used in the application. In this activity, there are two services: `database` and `app`. The `database` service runs MariaDB, while the `app` service runs Nextcloud. Docker Compose uses these settings to create and run the containers.

## How did the Nextcloud app container know how to find the database container?

The Nextcloud app uses the `MYSQL_HOST` environment variable to find the database container. In the YAML file, it is set to:

`MYSQL_HOST=database`

The name `database` matches the database service name under `services:`. Docker Compose allows the containers to communicate using their service names, so the Nextcloud container knows that `database` is where the MariaDB server is running.

## Difference between docker run and docker-compose up -d

The `docker run` command is used to create and run a single container with its settings given in the command. In Mission 4, it was used to run a container manually.

On the other hand, `docker-compose up -d` is used to start multiple containers based on the settings written in a `docker-compose.yml` file. It is easier for applications with multiple containers because their configuration is already written in one file. The `-d` option runs the containers in the background.
