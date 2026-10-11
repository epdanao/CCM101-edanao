# Laboratory 07: Cloud Operations Engineer

## Mission Overview

This laboratory activity focused on monitoring a Linux server and observing the performance of a web application using Docker. I used the KillerCoda Ubuntu Playground to check system resources, deploy an Nginx web server, generate website requests, examine application logs, and monitor container resource consumption. The purpose of this mission was to understand how Cloud Operations Engineers check server health, identify errors, and monitor applications to help maintain reliable services.

## Objectives

- Check the server's RAM usage and available disk storage.
- Observe CPU activity and running processes using Linux commands.
- Deploy an Nginx web server in a Docker container.
- Generate HTTP requests using the `curl` command.
- Identify a 404 Not Found response from a nonexistent webpage.
- Retrieve and analyze application logs using Docker.
- Monitor container CPU, memory, and network activity using `docker stats`.
- Document the results and evidence in Markdown and GitHub.

## Monitoring Commands Executed

| Command | Purpose |
|---|---|
| `free -h` | Displays total, used, free, and available memory. |
| `df -h /` | Checks the total and available storage of the root file system. |
| `top` | Displays CPU activity, memory usage, and running processes. |
| `docker run -d --name clientwebsite -p 8080:80 nginx` | Deploys the Nginx web server in the background and maps port 8080 to port 80. |
| `docker ps` | Checks the status of running Docker containers. |
| `curl http://localhost:8080` | Sends an HTTP request to the Nginx website. |
| `curl http://localhost:8080/hidden-admin-page` | Tests a nonexistent page and generates a 404 response. |
| `docker logs clientwebsite` | Displays the container's application logs. |
| `docker stats` | Monitors the container's CPU, memory, network, and block I/O usage in real time. |

## Skills Learned

Through this laboratory activity, I learned how to check the health of a Linux server and monitor the resources used by a Docker container. I practiced deploying an Nginx web server, sending HTTP requests, and identifying successful and failed responses. I also learned that application logs help administrators investigate errors, while Docker statistics provide information about CPU and memory consumption. These skills are useful for identifying possible performance problems and understanding how to maintain a reliable web application.
