# Laboratory 08: Cloud Security Engineer

## Mission Overview

This laboratory focuses on securing an Ubuntu server using UFW (Uncomplicated Firewall) and protecting a web application running in an Nginx container on port 8080.

## Objectives

- Understand the Principle of Least Privilege and attack surface.
- Audit active network ports.
- Configure UFW with a Default Deny policy.
- Allow SSH and TCP port 8080.
- Verify firewall rules and test the web application.

## Commands Executed

### Deploy the Nginx Container
```bash
docker run -d --name secure-web-app -p 8080:80 nginx
```

### Test the Web Application
```bash
curl http://localhost:8080
```

### Configure the Firewall
```bash
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw allow 8080/tcp
```

### Verify Firewall Status
```bash
sudo ufw status verbose
sudo ufw status numbered
```

## Skills Learned

- Deploying an Nginx web server using Docker.
- Checking web application responses using curl.
- Configuring host-based firewall rules with UFW.
- Applying the Default Deny policy.
- Managing SSH and web application access.
- Documenting technical procedures using Markdown.
