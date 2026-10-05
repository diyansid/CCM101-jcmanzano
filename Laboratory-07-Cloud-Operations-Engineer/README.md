# Laboratory 07 - Cloud Operations Engineer

## Mission Overview

This laboratory activity focused on monitoring the health and performance of a Linux server and a containerized Nginx web application. The activity involved checking system resources, generating web traffic, analyzing application logs, and monitoring real-time container metrics.

## Objectives

- Monitor host CPU, memory, and disk resources.
- Deploy an Nginx web server using Docker.
- Generate HTTP traffic using the `curl` command.
- Analyze application logs using `docker logs`.
- Monitor container CPU and memory usage using `docker stats`.
- Document system health and observability data using Markdown.

## Monitoring Commands Executed

```bash
free -h
df -h /
top
docker run -d --name client-website -p 8080:80 nginx
curl http://localhost:8080/
curl http://localhost:8080/hidden-admin-page
docker logs client-website
docker stats
