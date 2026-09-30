# Docker Compose Guide

## What does the `services:` block do?

The `services:` block defines the containers that make up the application. In this project, it contains two services: `database` for the MariaDB container and `app` for the Nextcloud container. Each service has its own image, settings, and configuration.

## How does the Nextcloud app find the database container?

The Nextcloud app uses the `MYSQL_HOST` environment variable to find the database container. In the YAML file, it is set to `database`:

```yaml
MYSQL_HOST: database
```

The name `database` matches the database service name in the Compose file. Docker Compose creates a network for the services, allowing the Nextcloud container to communicate with the MariaDB container using the service name.

## `docker run` vs. `docker-compose up -d`

The `docker run` command is mainly used to create and start an individual container. It is useful when deploying a simple application that only needs one container.

The `docker-compose up -d` command uses the `docker-compose.yml` file to create and start multiple related containers together. The `-d` option runs the containers in the background, allowing the terminal to be used for other commands.
