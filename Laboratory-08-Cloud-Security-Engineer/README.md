# Laboratory 08 - Cloud Security Engineer

## Mission Overview

This laboratory activity focused on securing an Ubuntu server using the Uncomplicated Firewall (UFW). The mission involved deploying an Nginx web application, configuring firewall policies, and managing network ports to reduce security risks.

## Objectives

- Understand the Principle of Least Privilege.
- Identify and reduce a server's attack surface.
- Deploy an Nginx web application using Docker.
- Configure UFW firewall rules.
- Apply a Default Deny policy.
- Allow SSH and HTTP traffic through specific ports.
- Document cloud security practices using Markdown.

## Commands Executed

```bash
docker run -d --name secure-web-app -p 8080:80 nginx
docker ps
curl -I http://localhost:8080/

sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose

sudo ufw allow 8080/tcp
sudo ufw status numbered

curl -I http://localhost:8080/
```

## Skills Learned

- Deploying containerized web applications using Docker.
- Understanding network security principles.
- Configuring firewall rules in Linux.
- Restricting unauthorized incoming connections.
- Managing SSH and web application ports.
- Verifying firewall configurations.
- Applying the principle of defense in depth.
- Documenting security configurations in Markdown.
