# Multi-Tier Architecture

## Two-Tier Architecture

A two-tier architecture is a system design where an application is separated into two main components: the application or web tier and the database tier. These two components communicate with each other to provide the complete functionality of the system.

## Web/Application Tier

The Web/Application Tier is responsible for displaying the user interface and handling HTTP requests from users. In this laboratory activity, Nextcloud acts as the application tier that users access through a web browser.

## Database Tier

The Database Tier is responsible for storing and managing persistent data used by the application. In this deployment, MariaDB stores information such as user accounts, settings, and file metadata required by Nextcloud.

## Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage, maintain, and troubleshoot. It also allows each service to be updated or restarted independently without affecting the other service.
