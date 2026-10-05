# Docker Compose Guide

## What does the `services:` block do?

The `services:` block defines the different containers that are part of the Docker Compose application. In this activity, it contains two services: the MariaDB database container and the Nextcloud application container. Each service includes its own image, environment variables, ports, and other configuration settings.

## How did the Nextcloud app container find the database container?

The Nextcloud app container connects to the MariaDB container using the `MYSQL_HOST` environment variable.

In the Compose file, the value is:

`MYSQL_HOST=database`

The word `database` matches the service name of the MariaDB container. Docker Compose automatically creates a network for the services, allowing the Nextcloud container to communicate with the database container using the service name.

## Difference Between `docker run` and `docker-compose up -d`

The `docker run` command is usually used to create and start a single container manually. The container settings such as ports, environment variables, and image names are written directly in the command.

The `docker-compose up -d` command uses a `docker-compose.yml` file to create and start multiple containers at the same time. It is more convenient for multi-container applications because the entire setup is defined in one configuration file.

The `-d` option runs the containers in detached mode, which means they continue running in the background.
