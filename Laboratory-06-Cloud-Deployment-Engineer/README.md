# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

This laboratory activity focused on deploying a multi-container private cloud storage application using Docker Compose. The deployment used Nextcloud as the web application and MariaDB as the database service.

## Objectives

- Understand the concept of a multi-tier application architecture.
- Learn the purpose and structure of a `docker-compose.yml` file.
- Use the Nano text editor to create configuration files.
- Deploy Nextcloud and MariaDB using Docker Compose.
- Understand Infrastructure as Code concepts.
- Document the deployment process using Markdown.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
