# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

In this laboratory, I deployed a multi-tier cloud storage application using Docker Compose. The application used Nextcloud as the web application and MariaDB as its database. Instead of setting up each container separately, I used a `docker-compose.yml` file to configure and deploy the whole application stack.

## Objectives

* Understand how multi-tier applications are structured.
* Create a Docker Compose configuration file.
* Deploy Nextcloud and MariaDB using multiple containers.
* Use Docker Compose to manage the application stack.
* Access the Nextcloud web interface through port 8080.
* Document the deployment process using Markdown.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
ls
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

* Creating and editing YAML configuration files.
* Deploying multiple containers using Docker Compose.
* Understanding the purpose of application and database containers.
* Connecting containers through Docker Compose service names.
* Using environment variables to configure containers.
* Checking container status and stopping a multi-container application.
* Documenting cloud deployment steps using Markdown.

