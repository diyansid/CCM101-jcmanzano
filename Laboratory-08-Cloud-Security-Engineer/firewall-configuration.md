# Firewall Configuration

## Overview

In this laboratory activity, I configured the Uncomplicated Firewall (UFW) on an Ubuntu server to protect a containerized Nginx web application. The firewall was configured to block incoming traffic by default while allowing authorized SSH connections and web traffic on port 8080.

## Allowing SSH Access

The following command was used to allow SSH connections:

```bash
sudo ufw allow ssh
```

This rule allows administrators to connect remotely to the server through SSH on port 22.

## Configuring the Default Deny Policy

The following commands were used to configure the firewall's default policies:

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

These commands block incoming connections by default while allowing outgoing traffic.

## Enabling the Firewall

The firewall was activated using:

```bash
sudo ufw enable
```

The firewall status was verified using:

```bash
sudo ufw status verbose
```

## Allowing Port 8080

The following command was used to allow incoming TCP traffic on port 8080:

```bash
sudo ufw allow 8080/tcp
```

The configured firewall rules were verified using:

```bash
sudo ufw status numbered
```

This rule allows web traffic through port 8080, which is used by the Nginx application.

## Importance of Allowing SSH Before Enabling UFW

If I enabled UFW before allowing SSH, the firewall could block incoming SSH connections and prevent administrators from remotely accessing the server.

## Conclusion

This activity helped me understand how firewall rules can reduce security risks by restricting unnecessary network traffic while allowing the services needed by legitimate users.
